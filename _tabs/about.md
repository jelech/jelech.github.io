---
title: 个人介绍
icon: fas fa-info-circle
order: 4
---
<div class="tab-buttons">
  <button data-tab="1" class="active">中文</button> | <button data-tab="2">En</button>
</div>

---

<div class="tab-content">
  <div id="tab-2" class="tab">
{% capture tab1_content %}
> 👋 Hi, I'm Jelech!
{: .prompt-tip }

👨‍💻 I'm a Backend Engineer with four years of professional experience. I specialize in **Golang** and have a robust skill set that includes **Python**, **Docker**, relational and NoSQL databases, game server development, and AI-enhanced engineering projects.

🔭 I’m currently working on:
- **lego**: A robust game server framework designed to handle high loads and provide real-time interactions.
- **cServer**: A back-end server written purely in C for performance-critical applications.
- **next-c**: A versatile data collection and scheduling platform that streamlines processes across various data sources.
- **pangolin-swaper**: A high-performance, distributed system for multi-source data transfer, ensuring efficient and reliable data handling.
- [more](https://www.github.com/jelech)



---

🌱 I’m currently learning more about cloud architectures and advanced machine learning models to enhance my backend development skills and integrate more AI features into my projects.

🎮 In my free time, I love coding personal projects, gaming, traveling, and making new friends all around the globe!

📫 How to reach me: Visit my blog at [www.jelech.top](https://www.jelech.top) or [jelech@hotmail.com](email://jelech@hotmail.com).

---

🌍 **Outreach:**
- 📝 Contributing to open-source projects on GitHub, including:
  - [machinery](https://github.com/RichardKnop/machinery): A high-performance task queue and distributed workflow engine.
  - [gorm](https://github.com/go-gorm/gorm): A robust ORM library for Golang, handling relational database interactions.
  - [imgProxy](https://github.com/imgproxy/imgproxy): A fast and secure image processing server, designed for high-scale web solutions.

---

💼 **Skills & Expertise:**
- **Languages**: Golang, Python
- **Technologies**: Docker, Kubernetes, Ray
- **Databases**: MySQL, MongoDB
- **Areas**: Data Systems, Game Server Development, AI-Enhanced Engineering
- Some other less commonly used technologies

---

🤝 **Let's Connect!**

I'm always open to connecting with like-minded individuals and exploring new collaborations. Feel free to reach out if you're interested in coding, gaming, or just want to chat and make a new friend!

Thanks for stopping by, and don't hesitate to get in touch!

    {% endcapture %}
    {{ tab1_content | markdownify }}
  </div>
  <div id="tab-1" class="tab active">
  {% capture tab1_content %}

> 👋 你好, 我叫Jelech
{: .prompt-tip }

👨‍💻 我是一名后端工程师，从2020年工作至今。专精于 **Golang**，并拥有丰富的技能，包括 **Python**、**Docker**、关系型和NoSQL**数据库**、**游戏服务器**开发以及RAG相关**AI工程项目**。

🔭 我曾经开发维护的项目：
- **lego**：一个强大的游戏服务器框架，设计用于处理高负载并提供实时交互。
- **cServer**：一个纯C语言编写的后端服务器，专为性能关键的应用设计。
- **next-c**：一个多功能数据采集和调度平台，简化了跨各种数据源的流程。
- **pangolin-swaper**：一个高性能的分布式系统，用于多源数据传输，确保数据处理的高效和可靠性。
- [更多项目](https://www.github.com/jelech)

---

🌱 我正在学习更多关于云架构和高级机器学习模型的知识，以提升我的后端开发技能，并将更多的AI特性整合到我的项目中。

🎮 在空闲时间，我喜欢开发个人项目、玩游戏、旅行，并结交来自世界各地的新朋友！

📫 如何联系我：访问我的博客 [www.jelech.top](https://www.jelech.top) 或者邮箱联系 [jelech@hotmail.com](email://jelech@hotmail.com)。

---

🌍 **对外贡献**：
- 📝 为以下GitHub开源项目做贡献：
  - [machinery](https://github.com/RichardKnop/machinery)：一个高性能的任务队列和分布式工作流引擎。
  - [gorm](https://github.com/go-gorm/gorm)：一个强大的Golang ORM库，处理关系型数据库交互。
  - [imgProxy](https://github.com/imgproxy/imgproxy)：一个快速且安全的图像处理服务器，专为大规模网络解决方案设计。

---

💼 **技能与专长**：
- **编程语言**：Golang、Python、Lua
- **技术栈**：Docker、K8s、Ray
- **数据库**：MySQL、MongoDB、Redis、Opensearch、RocketMQ
- **领域**：数据系统、传统web服务、游戏服务器开发、AI工程
- 其他一些较少使用的技术

---

🤝 **一起玩！**

如果你对编程、游戏感兴趣，或只是想聊聊并结交新朋友，请随时联系我！

感谢你的到访！

  {% endcapture %}
  {{ tab1_content | markdownify }}
  </div>
</div>

<script>
  const buttons = document.querySelectorAll('.tab-buttons button');
  const tabs = document.querySelectorAll('.tab');

  buttons.forEach(button => {
    button.addEventListener('click', function() {
      const tabId = this.getAttribute('data-tab');

      // Remove active class from all buttons and tabs
      buttons.forEach(btn => btn.classList.remove('active'));
      tabs.forEach(tab => tab.classList.remove('active'));

      // Add active class to the clicked button and corresponding tab
      this.classList.add('active');
      document.getElementById('tab-' + tabId).classList.add('active');
    });
  });
</script>

<style>
  .tab {
    display: none;
  }
  .tab.active {
    display: block;
  }
  .tab-buttons button {
    cursor: pointer;
    width: 60px;
    border: none;
    background-color: #fff;
    border-radius: 5px;
  }
  .tab-buttons button.active {
    background-color: #007bff;
    color: white;
  }
</style>

