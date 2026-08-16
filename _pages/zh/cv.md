---
layout: archive
title: "简历"
permalink: /zh/cv/
lang: zh
author_profile: true
redirect_from:
  - /zh/resume
---

<!-- 编辑说明：本页为中文简历，英文版对应 _pages/cv.md。论文/报告/教学三节自动从对应目录中 lang: zh 的条目生成。 -->

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

教育经历
======
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>翻译学与口译研究博士</strong>（英语语言文学），上海外国语大学，上海</span><span class="cv-item__date">预计 2028 年 6 月毕业</span></summary>
  <div class="cv-item__body"><ul>
    <li>博士论文选题：<i>Viewers&rsquo; Neurocognitive Processing of Errors in Raw Machine-Translated Subtitles</i></li>
    <li>导师：肖维青教授</li>
    <li>GPA 3.94/4.0 | 主修课程：认知语言学（95）、语料库语言学（90）、Python 编程与语言数据开发（92）、数字传播与视觉设计（90）</li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>翻译硕士</strong>（医学翻译方向），重庆医科大学，重庆</span><span class="cv-item__date">2020 年 9 月–2023 年 6 月</span></summary>
  <div class="cv-item__body"><ul>
    <li>硕士论文：多模态话语分析视角下纪录片《武汉战疫纪》的中英字幕翻译</li>
    <li>导师：LUO Ruifeng 教授 <!-- TODO: 请补中文姓名 --></li>
    <li>平均分 90.3/100 | 主修课程：翻译理论（98）、医学英语（96）、文学翻译（95）、多元统计分析（95）、口译理论与实践（94）、专题口译（93）、同声传译（91）、医学翻译（89）</li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>翻译学学士</strong>，西华大学，成都</span><span class="cv-item__date">2016 年 9 月–2020 年 6 月</span></summary>
  <div class="cv-item__body"><ul>
    <li>学士论文："Reshaping Translation Approaches to Unideal Texts: Translators' Emotional Orientation towards Text User"</li>
    <li>导师：GONG Xiaoping 教授 <!-- TODO: 请补中文姓名 --></li>
    <li>获评优秀毕业论文</li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>交换学习</strong>，佐治亚学院与州立大学，美国佐治亚州</span><span class="cv-item__date">2018 年 1–5 月</span></summary>
  <div class="cv-item__body"><ul>
    <li>GPA 4.0/4.0 | 校长名单</li>
    <li>课程：经济学与社会（A，以免考取得）、英语写作 I（A）、美国语言与文化导论（A）、世界区域地理（A）</li>
  </ul></div>
</details>

研究与教学兴趣
======
* 视听翻译与媒体无障碍
* 认知翻译与口译研究
* 翻译技术、生成式 AI 与伦理

论文
======
  <ul>{% for post in site.publications reversed %}
    {% if post.lang == 'zh' %}
      {% include archive-single-cv.html %}
    {% endif %}
  {% endfor %}</ul>

学术报告
======
  <ul>{% for post in site.talks reversed %}
    {% if post.lang == 'zh' %}
      {% include archive-single-talk-cv.html  %}
    {% endif %}
  {% endfor %}</ul>

教学
======
{% for post in site.teaching reversed %}
  {% if post.lang == 'zh' %}
    {% include archive-single-teaching-cv.html %}
  {% endif %}
{% endfor %}

科研经历
======
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>项目负责人</strong>，《人机协作下的 AI 翻译：应用边界与成效评估》，上海外国语大学"致远计划"企业出海项目</span><span class="cv-item__date">2026 年 7–9 月</span></summary>
  <div class="cv-item__body"><ul>
    <li>带领 12 人团队（本科、硕士、博士皆有）对三家公司开展 AI 翻译工作流的多案例研究，完成 15 场余深度访谈，并执笔 5 万字研究执行方案。</li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>研究助理</strong>，国家社会科学基金项目《认知工效学视角下的译后编辑过程实证研究》（21BYY063）</span><span class="cv-item__date">2021–2024</span></summary>
  <div class="cv-item__body"><ul>
    <li>用 R 完成眼动数据建模与统计分析。</li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>课题组成员</strong>，上外"导师学术引领计划"项目《计算机辅助翻译环境下的译后编辑表现》（2024DSYL018）</span><span class="cv-item__date">2024–2026</span></summary>
  <div class="cv-item__body"><ul>
    <li>为实验翻译材料设计了一套错误加权评分体系。</li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>课题组成员</strong>，虹口区教育局课题《AI 辅助初中英语翻译教学创新实践》，上海</span><span class="cv-item__date">2025–2027</span></summary>
  <div class="cv-item__body"><ul>
    <li>开发了面向初中英语翻译教学的 AI 训练平台，包括教学系统设计和教学案例集。</li>
  </ul></div>
</details>

国际交流
======
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>波兰亚当·密茨凯维奇大学 MC2 Lab 第三届认知翻译与口译研究国际暑期学校</strong>，Poznań</span><span class="cv-item__date">2025 年 7 月</span></summary>
  <div class="cv-item__body"><ul>
    <li>授课语言：英语 | 125 学时（5 ECTS 学分），含讲授、小组与个人辅导</li>
    <li>由 Ricardo Muñoz Martín 教授与 Bogusława Whyatt 教授联合主持</li>
    <li>模块：认知翻译与口译研究（R. Muñoz Martín 教授）、心理语言学与翻译心理学（B. Whyatt 教授）、翻译技术与伦理（J. Moorkens 教授）、研究方法（A.M. Rojo López 教授）、统计学（C.D. Mellinger 教授）、学术交流与发表（A. Chmiel 教授）</li>
    <li>经竞争性遴选录取</li>
    <li>结业论文 "Behind the Consulting Rooms: Cognitive Process of Student and Professional Translators in AI-mediated Adaptation of Pediatric Developmental Scale" 经 TREC（翻译实证与实验研究主题网络）同行评议，获<strong>最佳论文第二名</strong></li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>交换学习</strong>，美国佐治亚学院与州立大学，美国佐治亚州</span><span class="cv-item__date">2018 年 1–5 月</span></summary>
  <div class="cv-item__body"><ul>
    <li>GPA 4.0/4.0 | 校长名单</li>
    <li>课程：经济学与社会（A，获免考）、英语写作 I（A）、美国语言与文化导论（A）、世界区域地理（A）</li>
  </ul></div>
</details>

相关职业经历
======
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>沙龙组织者</strong>，上外–莱斯特翻译研究沙龙，上海外国语大学，上海</span><span class="cv-item__date">2024 年 10 月–2025 年 12 月</span></summary>
  <div class="cv-item__body"><ul>
    <li>组织月度沙龙 11 期，累计 300 余人次参与，促成上外与莱斯特大学等地研究者的对话</li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>撰稿人与编辑</strong>，"翻译技术教育与研究"微信公众号，线上</span><span class="cv-item__date">2023 年 10 月–2024 年 12 月</span></summary>
  <div class="cv-item__body"><ul>
    <li>撰写翻译技术原创文章；获评"优秀编辑"（2024 年 2 月）</li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>专职译员/口译员</strong>，重庆市人民政府外事办公室翻译中心，重庆</span><span class="cv-item__date">2022 年 8 月–2024 年 6 月</span></summary>
  <div class="cv-item__body"><ul>
    <li>为百余场活动提供交替传译和同声传译，服务对象包括市领导、各国驻华使节及领事官员</li>
    <li>为"一带一路"科技交流大会、中新金融峰会、中国国际智能产业博览会（智博会）等国际峰会翻译会议材料</li>
    <li>参与重庆市公共场所英文标识规范化工作，为市外事期刊《重庆与世界》供稿翻译</li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>翻译与本地化实习生</strong>，创思立信科技（EC Innovations）生命科学事业部，重庆</span><span class="cv-item__date">2022 年 2–8 月</span></summary>
  <div class="cv-item__body"><ul>
    <li>为强生、信达、再鼎、卫材、山德士、CDS 等 15 余家全球制药企业提供中英本地化服务</li>
    <li>累计审校约 20 万词、翻译约 2 万词、审读约 3.5 万词，内容涵盖临床、药理与法规文件</li>
  </ul></div>
</details>
<details class="cv-item">
  <summary><span class="cv-item__head"><strong>翻译与审校实习生</strong>，快译商城（QTransMall.com），成都</span><span class="cv-item__date">2021 年 7–8 月</span></summary>
  <div class="cv-item__body"><ul>
    <li>翻译、编辑与质检合计约 20 万词，领域涉及生物医药、消费电子、法律合同、政府文书与财务报告</li>
  </ul></div>
</details>

获奖情况
======
* 上海外国语大学优秀学生奖，2024–2025
* 海峡两岸口译大赛：西南赛区一等奖（第一名）、大陆总决赛二等奖、全国总决赛季军，2022–2023
* 国家奖学金，教育部，2019

专业进修
======
* 第四届 IATIC 认知翻译与口译研究与学术写作工作坊，IATIC，武汉理工大学，2026 年 7 月
* 应用语言学中的 Q 方法论：理论、实践与实证研究，外语教学与研究出版社、北京语言大学，2025 年 11 月
* 第二届 IATIC 认知翻译与口译研究与学术写作工作坊，IATIC，武汉理工大学 & 澳门大学，2024 年 7 月
* AI 时代口译教学创新圆桌研讨，澳门大学，2023 年 6 月
* 医学翻译、口译与语言服务培训课程，广东外语外贸大学，2022 年 8 月
* Python 数据分析，上海交通大学，2022 年 7 月
* 影视字幕翻译技术工作坊，1sj.tv & Lingotek，2022 年 5 月
* 语料库处理技术与语言资源管理工作坊，广东外语外贸大学，2022 年 1 月

技能与证书
======
* **语言**：中文（母语）、英语（专业八级）、西班牙语（初级）
* **证书**：CATTI 一级笔译（译审，中英最高等级）；CATTI 二级交替传译（中英）；TED 字幕注册译者
* **研究方法**：EEG 与眼动协同记录、语料库语言学、内容分析
* **编程**：Python（NLP、文本分析、数据可视化）、R（统计建模、文献计量）、JavaScript（前端、音频与实时处理、AI 集成）

学术与社区服务
======
* TED Translators 审校
* 上外–莱斯特翻译研究沙龙组织者（2024–2025）
* 知远·英文成长计划（面向残障人士的公益英语项目）志愿教师，为视障学习者讲授英语，2021
* 英国中文培优项目（#MEP）访华研学夏令营（Intensive Study in China Summer Camp）：线下助教（2019）、线上中文教师（2021）

<p class="cv-download"><button class="pub-dl" type="button" onclick="window.print()"><i class="fa-solid fa-download" aria-hidden="true"></i>下载简历（PDF）</button></p>
