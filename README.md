# Henry Murdock

### Announcements

<div class="announcement-list">
  <article class="announcement-item">
    <p class="announcement-date">8/25/2025</p>
    <p class="announcement-title">Started Masters Degree at UIUC</p>
    <p>Classes for Fall 2025:</p>
    <ul>
      <li>Manycore Parallel Algorithms (ECE 508)</li>
      <li>Distributed Systems (CS 425)</li>
      <li>Applied Machine Learning (CS 441)</li>
    </ul>
  </article>

  <article class="announcement-item">
    <p class="announcement-date">5/2025</p>
    <p class="announcement-title">Started full-time SWE for the summer with KLA Computational Physics</p>
    <p>Working on computational acceleration of electron optics simulations.</p>
  </article>

  <article class="announcement-item">
    <p class="announcement-date">5/2025</p>
    <p class="announcement-title">Graduated from Michigan State University</p>
    <p>B.S. in Computer Science, GPA: 4.0/4.0.</p>
  </article>

  <article class="announcement-item">
    <p class="announcement-date">5/2025</p>
    <p class="announcement-title">Completed Spring 2025</p>
    <p>Notable classes: Performance Engineering and graduate-level DSA. The Performance Engineering course mirrors MIT's course by Charles E. Leiserson.</p>
  </article>

  <article class="announcement-item">
    <p class="announcement-date">4/2025</p>
    <p class="announcement-title">Accepted M.C.S offer from University of Illinois Urbana-Champaign</p>
  </article>

  <article class="announcement-item">
    <p class="announcement-date">4/2025</p>
    <p class="announcement-title">Accepted to University of Michigan Computer Science M.S. program</p>
  </article>

  <article class="announcement-item">
    <p class="announcement-date">3/2025</p>
    <p class="announcement-title">Accepted to University of Illinois Urbana-Champaign M.C.S. program</p>
  </article>

  <article class="announcement-item">
    <p class="announcement-date">3/2025</p>
    <p class="announcement-title">Accepted to Michigan State University Computer Science M.S. program</p>
  </article>

  <article class="announcement-item">
    <p class="announcement-date">12/2024</p>
    <p class="announcement-title">Completed AbbVie capstone project</p>
    <p>Analysis of biphasic solutions using computer vision.</p>
  </article>

  <article class="announcement-item">
    <p class="announcement-date">9/2024</p>
    <p class="announcement-title">Accepted KLA offer for SWE P1 (Summer 2025)</p>
    <p>Includes MCS sponsorship and a post-graduation P2 position.</p>
  </article>

  <article class="announcement-item">
    <p class="announcement-date">5/2024</p>
    <p class="announcement-title">Started second SWE internship at KLA Computational Physics</p>
  </article>
</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  var badgeMap = {
    "CUDA": "https://img.shields.io/badge/CUDA-76B900?logo=nvidia&logoColor=white",
    "C/C++": "https://img.shields.io/badge/C%2FC%2B%2B-00599C?logo=cplusplus&logoColor=white",
    "Python": "https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white",
    "GPU": "https://img.shields.io/badge/GPU-111827?logo=nvidia&logoColor=white"
  };

  var lists = document.querySelectorAll(".social-media-list");
  lists.forEach(function (list) {
    var items = list.querySelectorAll("li");
    if (items.length < 3) return;

    var skillItems = [];
    for (var i = 2; i < items.length; i++) {
      var li = items[i];
      var link = li.querySelector("a");
      if (!link) continue;
      skillItems.push(link.textContent.trim());
      li.remove();
    }

    if (!skillItems.length) return;

    var section = document.createElement("div");
    section.className = "skills-badge-section";

    var heading = document.createElement("p");
    heading.className = "skills-badge-title";
    heading.textContent = "Skills";
    section.appendChild(heading);

    var row = document.createElement("div");
    row.className = "skills-badge-row";

    skillItems.forEach(function (label) {
      var badge = document.createElement("span");
      badge.className = "skill-badge";

      var badgeUrl = badgeMap[label];
      if (badgeUrl) {
        var img = document.createElement("img");
        img.className = "skill-badge-image";
        img.src = badgeUrl;
        img.alt = label + " badge";
        img.loading = "lazy";
        badge.appendChild(img);
      } else {
        badge.classList.add("skill-badge--text");
        badge.textContent = label;
      }

      row.appendChild(badge);
    });

    section.appendChild(row);
    list.insertAdjacentElement("afterend", section);
  });
});
</script>

### Education

<div class="announcement-list">
  <article class="announcement-item">
    <p class="announcement-date">8/2025 - 12/2026 (Expected)</p>
    <p class="announcement-title">University of Illinois Urbana-Champaign</p>
    <p>Professional Master of Computer Science.</p>
  </article>

  <article class="announcement-item">
    <p class="announcement-date">8/2021 - 5/2025</p>
    <p class="announcement-title">Michigan State University</p>
    <p>B.S. Computer Science, GPA: 4.0/4.0.</p>
  </article>
</div>

### Experience

<div class="announcement-list">
  <article class="announcement-item">
    <p class="announcement-date">5/2025 - Present</p>
    <p class="announcement-title">Software Engineer, KLA Computational Physics</p>
    <p>Accepted KLA sponsorship for a masters degree, with full-time summer and part-time school-year work. Focused on accelerating electron-optics simulation for scanning electron microscopes. Moved Coulomb N-body electron interaction to GPU using a tree-based method, scaling particles per GPU from 10<sup>5</sup> to 10<sup>10</sup>.</p>
  </article>

  <article class="announcement-item">
    <p class="announcement-date">5/2024 - 5/2025</p>
    <p class="announcement-title">Software Intern, KLA Computational Physics</p>
    <p>Worked in skunkworks on a new SEM physics simulation program, including refactoring and infrastructure for simplified core models. Reached 800x speedup in secondary electron yield emission generation using Numba CUDA. The project became fully funded and continued part-time during senior year.</p>
  </article>

  <article class="announcement-item">
    <p class="announcement-date">5/2023</p>
    <p class="announcement-title">Software Intern, KLA SW Infra</p>
    <p>Developed Apache Airflow pipelines to deploy ML models on Kubernetes with GPU support and dynamic training-instance control, including cluster setup and NVIDIA GPU Operator integration.</p>
  </article>
</div>
