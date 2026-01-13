---
permalink: /
title: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
    
---

Hi! I am a second-year PhD student in Economics at Northwestern University. My interests are in macroeconomics, particularly in short- to medium-run fluctuations.

Before coming to Northwestern, I received my undergraduate and postgraduate degrees from St. John's College, University of Cambridge. I was lucky enough to be funded by [Nagase Bros., Inc.](https://www.bloomberg.com/profile/company/9733:JP) during the four years there. 

In my free time, I like to watch (and sometimes play) rugby union. I normally play halfback. I have also played rugby league on a few occasions. I go by Hiro.

<span style="color:blue">*My random Nikkei stock pick for you*</span>: 
<span id="random-row"></span>
<button id="sanity">Sanity check</button>
## Contact
email: [hiroakiendo2030[at]u.northwestern.edu](mailto:hiroakiendo2030@u.northwestern.edu)

github: [https://github.com/hiroendo1014/](https://github.com/hiroendo1014/)

![](/images/about.jpg){: .float-photo }

<script>
document.getElementById("sanity").addEventListener("click", async () => {
  alert("JS is running ✅");

  const url = "{{ '/files/misc/nikkei.csv' | relative_url }}";
  alert("Fetching: " + url);

  try {
    const r = await fetch(url);
    alert("Fetch status: " + r.status);

    const text = await r.text();
    alert("First 200 chars:\n" + text.slice(0, 200));

    document.getElementById("random-row").textContent = "Loaded ✅";
  } catch (e) {
    alert("Error: " + e);
  }
});
  
async function displayRandomRow(csvUrl, elementId) {
  const response = await fetch(csvUrl);
  const text = await response.text();

  // Handle different line endings
  const lines = text.trim().split(/\r?\n/);

  const headers = lines[0].split(",");
  const rows = lines.slice(1);

  if (rows.length === 0) return;

  const randomLine = rows[Math.floor(Math.random() * rows.length)];
  const values = randomLine.split(",");

  const row = Object.fromEntries(
    headers.map((h, i) => [h.trim(), values[i]?.trim()])
  );

  document.getElementById(elementId).textContent =
    `${row.Code} — ${row.Company}`;
}

// Call after definition
displayRandomRow(
  "{{ '/files/misc/nikkei.csv' | relative_url }}",
  "random-row"
);
</script>
