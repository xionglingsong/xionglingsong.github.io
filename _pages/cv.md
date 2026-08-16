---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

<!-- 编辑说明：本页为英文 CV。中文版对应 _pages/zh/cv.md。
     Publications / Talks / Teaching 三节自动从 _publications、_talks、_teaching 目录生成。 -->

{% include base_path %}


<script>
  window.addEventListener('beforeprint', function () {
    document.querySelectorAll('details').forEach(function (d) {
      d.dataset.wasOpen = d.open; d.open = true;
    });
  });
  window.addEventListener('afterprint', function () {
    document.querySelectorAll('details').forEach(function (d) {
      if (d.dataset.wasOpen !== undefined) d.open = d.dataset.wasOpen === 'true';
    });
  });
</script>

Education
======
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>Ph.D.</strong> in Translation and Interpreting Studies (English Language and Literature), Shanghai International Studies University, Shanghai</span><span class="cv-item__date">expected Jun 2028</span></summary>
  <div class="cv-item__body"><ul>
    <li>Dissertation proposal: <i>Viewers&rsquo; Neurocognitive Processing of Errors in Raw Machine-Translated Subtitles</i></li>
    <li>Advisor: Professor Xiao Weiqing</li>
    <li>GPA: 3.94/4.0 | Key modules: Cognitive Linguistics (95), Corpus Linguistics (90), Python Programming and Linguistic Data Development (92), Digital Communication and Visual Design (90)</li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>M.TI.</strong> in Medical Translation, Chongqing Medical University, Chongqing</span><span class="cv-item__date">Sep 2020 &ndash; Jun 2023</span></summary>
  <div class="cv-item__body"><ul>
    <li>Thesis: &ldquo;Chinese&ndash;English Subtitle Translation of Documentary <i>The Lockdown: One Month in Wuhan</i> from the Perspective of Multimodal Discourse Analysis&rdquo;</li>
    <li>Advisor: Professor Luo Ruifeng</li>
    <li>Average score: 90.3/100 | Key modules: Translation Theory (98), Medical English (96), Literary Translation (95), Multivariate Statistical Analysis (95), Interpreting Theory and Practice (94), Thematic Interpreting (93), Simultaneous Interpreting (91), Medical Translation (89)</li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>B.A.</strong> in Translation and Interpreting, Xihua University, Chengdu</span><span class="cv-item__date">Sep 2016 &ndash; Jun 2020</span></summary>
  <div class="cv-item__body"><ul>
    <li>Thesis: &ldquo;Reshaping Translation Approaches to Unideal Texts: Translators&rsquo; Emotional Orientation towards Text User&rdquo;</li>
    <li>Advisor: Professor Gong Xiaoping</li>
    <li>Awarded Outstanding Graduation Thesis</li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>Exchange student</strong>, Georgia College &amp; State University, Georgia, USA</span><span class="cv-item__date">Jan &ndash; May 2018</span></summary>
  <div class="cv-item__body"><ul>
    <li>GPA: 4.0/4.0 | President&rsquo;s List</li>
    <li>Modules: Economics and Society (A, exam exemption earned), English Composition I (A), Introduction to American Language and Culture (A), World Regional Geography (A)</li>
  </ul></div>
</details>

Research and teaching interests
======
* Audiovisual translation and media accessibility
* Cognitive translation and interpreting studies
* Translation technology, generative AI, and ethics

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% if post.lang != 'zh' %}
      {% include archive-single-cv.html %}
    {% endif %}
  {% endfor %}</ul>

Talks
======
  <ul>{% for post in site.talks reversed %}
    {% if post.lang != 'zh' %}
      {% include archive-single-talk-cv.html  %}
    {% endif %}
  {% endfor %}</ul>

Teaching
======
{% for post in site.teaching reversed %}
  {% if post.lang != 'zh' %}
    {% include archive-single-teaching-cv.html %}
  {% endif %}
{% endfor %}

Research experience
======
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>Principal Investigator</strong>, <i>AI Translation in Human&ndash;Machine Collaboration: Application Boundaries and Efficacy Evaluation</i>, &ldquo;Zhiyuan Program&rdquo; grant (SISU fund for student-led research, enterprise-going-global track)</span><span class="cv-item__date">Jul &ndash; Sep 2026</span></summary>
  <div class="cv-item__body"><ul>
    <li>Led a 12-member cross-level team in a multi-case study of AI translation workflows at three companies, with 15+ in-depth interviews; authored a 50,000-character research execution protocol.</li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>Research Assistant</strong>, <i>Empirical Study on Post-Editing Processes from a Cognitive Ergonomics Perspective</i>, National Social Science Fund of China (Grant No. 21BYY063)</span><span class="cv-item__date">2021 &ndash; 2024</span></summary>
  <div class="cv-item__body"><ul>
    <li>Conducted eye-tracking data modeling and statistical analysis with R.</li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>Research Team Member</strong>, <i>Post-Editing Performance in Computer-Assisted Translation Environments</i>, SISU &ldquo;Supervisor Academic Leadership Program&rdquo; (Grant No. 2024DSYL018)</span><span class="cv-item__date">2024 &ndash; 2026</span></summary>
  <div class="cv-item__body"><ul>
    <li>Designed and implemented an error-weight scoring system for experimental translation materials.</li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>Research Team Member</strong>, <i>Innovative Practices in AI-Assisted Junior High School English Translation Teaching</i>, Hongkou District Education Bureau, Shanghai</span><span class="cv-item__date">2025 &ndash; 2027</span></summary>
  <div class="cv-item__body"><ul>
    <li>Developed an AI-powered translation training platform, including instructional system design and teaching case collections.</li>
  </ul></div>
</details>

International research and study
======
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>MC2 Lab&rsquo;s 3rd International Summer School on Cognitive Translation &amp; Interpreting Studies</strong>, Adam Mickiewicz University, Poznań, Poland</span><span class="cv-item__date">Jul 2025</span></summary>
  <div class="cv-item__body"><ul>
    <li>Language of instruction: English | 125 contact hours (5 ECTS credits), comprising lectures, group and individual tutorials</li>
    <li>Co-directed by Prof. Ricardo Muñoz Martín and Prof. Bogusława Whyatt</li>
    <li>Modules: Cognitive Translation &amp; Interpreting Studies (Prof. R. Muñoz Martín), Psycholinguistics and Translation Psychology (Prof. B. Whyatt), Translation Technology and Ethics (Prof. J. Moorkens), Research Methods (Prof. A.M. Rojo López), Statistics (Prof. C.D. Mellinger), Academic Communication and Publishing (Prof. A. Chmiel)</li>
    <li>Admitted through competitive application review</li>
    <li>Final paper &ldquo;Behind the Consulting Rooms: Cognitive Process of Student and Professional Translators in AI-mediated Adaptation of Pediatric Developmental Scale,&rdquo; awarded <strong>Second Best Paper</strong> following TREC (Thematic Network on Empirical and Experimental Research in Translation) peer review</li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>Exchange student</strong>, Georgia College &amp; State University, Georgia, United States</span><span class="cv-item__date">Jan &ndash; May 2018</span></summary>
  <div class="cv-item__body"><ul>
    <li>GPA: 4.0/4.0 | President&rsquo;s List</li>
    <li>Modules: Economics and Society (A, exam exemption earned), English Composition I (A), Introduction to American Language and Culture (A), World Regional Geography (A)</li>
  </ul></div>
</details>

Relevant professional experience
======
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>Seminar Organizer</strong>, SISU&ndash;Leicester Translation Studies Salon, Shanghai International Studies University, Shanghai</span><span class="cv-item__date">Oct 2024 &ndash; Dec 2025</span></summary>
  <div class="cv-item__body"><ul>
    <li>Organized 11 monthly sessions attracting 300+ attendees, facilitating dialogue between SISU and University of Leicester researchers and beyond</li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>Writer and Editor</strong>, Translation Technology Education and Research WeChat Account, Online</span><span class="cv-item__date">Oct 2023 &ndash; Dec 2024</span></summary>
  <div class="cv-item__body"><ul>
    <li>Authored original articles on translation technology; awarded &ldquo;Outstanding Editor&rdquo; (February 2024)</li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>In-house Translator and Interpreter</strong>, Chongqing Translation &amp; Interpretation Center, Foreign Affairs Office of Chongqing Municipal Government, Chongqing</span><span class="cv-item__date">Aug 2022 &ndash; Jun 2024</span></summary>
  <div class="cv-item__body"><ul>
    <li>Provided consecutive and simultaneous interpreting for 100+ events involving municipal leaders, foreign ambassadors, and consular officials</li>
    <li>Translated conference materials for international summits including the Belt and Road Science and Technology Exchange Conference, China-Singapore Financial Summit, and Smart China Expo</li>
    <li>Contributed to standardizing English signage in Chongqing&rsquo;s public spaces and translating content for the municipal foreign affairs journal <i>Chongqing and the World</i></li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>Translation and Localization Trainee</strong>, Life Sciences BU, EC Innovations, Chongqing</span><span class="cv-item__date">Feb &ndash; Aug 2022</span></summary>
  <div class="cv-item__body"><ul>
    <li>Delivered Chinese&ndash;English localization services for 15+ global pharmaceutical companies (CDS, JNJ, Innovent, Zai Lab, Eisai, Sandoz, etc.)</li>
    <li>Edited approximately 200,000 words, translated approximately 20,000 words, and proofread approximately 35,000 words of clinical, pharmacological, and regulatory documentation</li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>Translator and Proofreader Trainee</strong>, QTransMall.com, Chengdu</span><span class="cv-item__date">Jul &ndash; Aug 2021</span></summary>
  <div class="cv-item__body"><ul>
    <li>Translated, edited, and quality-checked approximately 200,000 words across domains including biomedicine, consumer electronics, legal contracts, government communications, and financial reporting</li>
  </ul></div>
</details>

Selected awards
======
* Outstanding Student Award, Shanghai International Studies University, 2024–2025
* Cross-Strait Interpreting Competition, 2022–2023 — First Prize (1st place, Southwest Regional Round); Second Prize (Mainland Final); Third Prize (National Grand Final)
* National Scholarship, Ministry of Education, China, 2019

Professional development
======
* The 4th IATIC Workshop on Cognitive Translation & Interpreting Research and Academic Writing, IATIC, Wuhan University of Technology, Jul 2026
* Q Methodology in Applied Linguistics: Theory, Practice, and Empirical Research, Foreign Language Teaching and Research Press & Beijing Language and Culture University, Nov 2025
* The 2nd IATIC Workshop on Cognitive Translation & Interpreting Research and Academic Writing, IATIC, Wuhan University of Technology & University of Macau, Jul 2024
* Roundtable Seminar on Innovations in Interpreter Training in the Era of AI, University of Macau, Jun 2023
* Medical Translation, Interpretation, and Language Service Training Course, Guangdong University of Foreign Studies, Aug 2022
* Data Analysis with Python, Shanghai Jiao Tong University, Jul 2022
* Film and Television Subtitle Translation Technology Workshop, 1sj.tv & Lingotek, May 2022
* Corpus Processing Technology and Language Resource Management Workshop, Guangdong University of Foreign Studies, Jan 2022

Skills and certifications
======
* **Languages**: Chinese (native), English (advanced, TEM-8), Spanish (elementary)
* **Certification**: CATTI Level 1 Translator and Reviewer (Chinese–English, highest tier); CATTI Level 2 Consecutive Interpreter (Chinese–English); Registered TED Talks Subtitler
* **Research methods**: EEG and eye-tracking co-registration, corpus linguistics, content analysis
* **Programming**: Python (NLP, text analysis, data visualization), R (statistical modeling, bibliometrics), JavaScript (front-end, audio and real-time processing, AI integration)

Academic and community service
======
* Reviewer, TED Translators
* Organizer, SISU–Leicester Translation Studies Salon (2024–2025)
* Volunteer English teacher for learners with visual impairments, Zhiyuan English Growth Program (a nonprofit English program for people with disabilities), 2021
* Teaching assistant (on-site, 2019) and Chinese teacher (online, 2021), UK Mandarin Excellence Programme (#MEP) Intensive Study in China Summer Camp

<p class="cv-download"><button class="pub-dl" type="button" onclick="window.print()"><i class="fa-solid fa-download" aria-hidden="true"></i>Download this CV as PDF</button></p>
