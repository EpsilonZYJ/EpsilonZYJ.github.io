---
permalink: /
title: "Yujie Zhou"
excerpt: "Yujie Zhou personal homepage."
description: "Yujie Zhou - Undergraduate in CS at HUST, interests in GNN, Graph Transformer, systems and databases."
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

I am currently an undergraduate student at *Huazhong University of Science and Technology*, majoring in Computer Science and Technology under the Experimental Program for Exemplary Engineer Education. Now I am researching in the field of GNN and Graph Transformer under the supervision of *Prof. [Kun He](https://scholar.google.com/citations?hl=zh-CN&user=YTQnGJsAAAAJ&view_op=list_works&sortby=pubdate)*. Additionally, I am also interested in computer systems and database systems.

- CV: [EN](https://epsilonzyj.github.io/blog/about/cv-en.pdf) ｜ [ZH-CN](https://epsilonzyj.github.io/blog/about/cv-zh-CN.pdf)

<!-- My research interest includes neural machine translation and computer vision. I have published more than 100 papers at the top international AI conferences with total <a href='https://scholar.google.com/citations?user=DhtAFkwAAAAJ'>google scholar citations <strong><span id='total_cit'>260000+</span></strong></a> (You can also use google scholar badge <a href='https://scholar.google.com/citations?user=DhtAFkwAAAAJ'><img src="https://img.shields.io/endpoint?url={{ url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=citations"></a>). -->

# 📖 Educations

<img class="jpg" src="/images/hust-logo.jpg" width="50pt"> Huazhong University of Science and Technology
<br>
- *Sept. 2023 - Jun. 2027*, Bachelor of Engineering in Computer Science and Technology, GPA: 4.68/5.00, Rank: **1**/30.

<img class="jpg" src="/images/nus-logo.jpg" width="50pt"> National University of Singapore
<br>
- *May. 2025 - Jul. 2025*, Summer Workshop on Deep Learning, School of Computing. Score: **A+**.

<!-- # 🔥 News
- *2022.02*: &nbsp;🎉🎉 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2022.02*: &nbsp;🎉🎉 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet.  -->

<!-- # 📝 Publications  -->

# 📝 Research

<div class='paper-box' markdown="1">

**Research on Efficient Heuristic Algorithms for Blocking Flow-shop Scheduling Problem**

- Developed a high-performance C++ solver for the Blocking Flow-shop Scheduling Problem (BFSP) utilizing an improved Discrete Invasive Weed Optimization (DIWO) algorithm.
- Engineered a hybrid algorithmic framework by integrating PF-NEH initialization and SRLS local search to enhance solution quality and convergence speed.
- Optimized the neighborhood evaluation function, successfully reducing computational complexity from O(mn²) to O(mn), which significantly accelerated the solving process.
- Validated the algorithm on Taillard’s benchmark instances, achieving superior precision with an Average Relative Percentage Deviation (ARPD) as low as 1.78%.
- Contributed to the design and implementation of core software modules and conducted extensive performance tuning.

[[Code]](https://github.com/yunbow30944/BFSP-DIWO)

</div>

<!-- <div class='paper-box'><div class='paper-box-image'><div><div class="badge">CVPR 2016</div><img src='images/500x300.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Deep Residual Learning for Image Recognition](https://openaccess.thecvf.com/content_cvpr_2016/papers/He_Deep_Residual_Learning_CVPR_2016_paper.pdf)

**Kaiming He**, Xiangyu Zhang, Shaoqing Ren, Jian Sun

[**Project**](https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=DhtAFkwAAAAJ&citation_for_view=DhtAFkwAAAAJ:ALROH1vI_8AC) <strong><span class='show_paper_citations' data='DhtAFkwAAAAJ:ALROH1vI_8AC'></span></strong>
- Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
</div>
</div>

- [Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet](https://github.com), A, B, C, **CVPR 2020** -->

# 🚀 Projects
<div class='paper-box' markdown="1">

**RISC-V Proxy Operating System Kernel**

- Developed a multi-core, concurrency-safe proxy OS kernel based on the RISC-V architecture using the Spike simulator.
- Implemented Sv39 virtual memory with Copy-on-Write (CoW) mechanisms, optimizing memory overhead through page table permission control and page reference counting.
- Engineered process management and scheduling modules (fork, yield, wait) utilizing Round-Robin scheduling and synchronization primitives like semaphores and spinlocks.
- Designed a Virtual File System (VFS) abstraction layer supporting comprehensive file operations, directories, links, and relative path resolution.
- Created an interactive Shell featuring command history and environment variables, while implementing kernel-supported pipes for IPC and dynamic multi-core background task scheduling.  

[[Code]](https://github.com/EpsilonZYJ/riscv-pke)

</div>
<div class='paper-box' markdown="1">

**RMDB Relational Database Management System**

- Implemented SQL lexical and syntax parsing based on Flex/Bison, constructed the AST, and completed semantic
analysis including column binding, type checking, and conditional expression validation.
- Built a rule-based query optimizer and a Volcano-model execution engine, supporting operators such as
predicate pushdown, projection pushdown, index selection, and join plan generation.
- Designed a page-based storage architecture, buffer pool, and B+ tree composite indexes, supporting
equality queries, range scans, and leftmost-prefix matching.
- Implemented transaction rollback and MVCC-based snapshot visibility control, and built a logging and recovery framework to support database crash recovery.

[[Code]](https://github.com/EpsilonZYJ/db2025-yoursql)

</div>
<div class='paper-box' markdown="1">

**Real-time Monitoring Robot System based on YOLOv7**

- Managed the collection, cleaning, and preprocessing of multi-class datasets (smoking, fighting, falling, littering) and fine-tuned the YOLOv7 framework to optimize detection accuracy and inference speed for specialized surveillance scenarios.
- Implemented a multi-model object detection system integrated with the SORT tracking algorithm to ensure stable target persistence in complex environments; developed a sliding window algorithm for video stream processing to enable effective recognition of continuous temporal behaviors.
- Designed and deployed an "End-Edge-Cloud" system architecture utilizing the MQTT protocol for efficient data transmission between robots and backend servers; built a comprehensive monitoring client using Dear PyGui to facilitate a seamless workflow from video input and model inference to real-time result visualization. 

[[Code]](https://github.com/EpsilonZYJ/NUS-SOC)

</div>

# 🎖 Honors and Awards
- *2024-2026* Outstanding Undergraduate in Term of Academic Performance (Top 1% at HUST)
- *2025.12* China National Scholarship (Top 0.2% nationwide)
- *2025.12* "Merit Student" of Huazhong University of Science and Technology
- *2024.12* "Merit Student" of Huazhong University of Science and Technology
- *2024.06* "Scholarship for Academic Excellence" of Huazhong University of Science and Technology

<!-- # 💬 Invited Talks
- *2021.06*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2021.03*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet.  \| [\[video\]](https://github.com/) -->

<!-- # 💻 Internships
- *2019.05 - 2020.02*, [Lorem](https://github.com/), China. -->