
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Cherrak Infinity ♾️ | المنصة العالمية المتطورة</title>
  <meta name="description" content="Cherrak Infinity ♾️ المنصة الذكية العالمية المعتمدة على الذكاء الاصطناعي.">
  <link rel="icon" href="https://cdn-icons-png.flaticon.com/512/4712/4712108.png">
  <style>
    *{margin:0;padding:0;box-sizing:border-box;font-family:'Poppins',sans-serif}
    body{
      background: radial-gradient(circle at top,#0b1220,#000);
      color:#fff;
      display:flex;
      flex-direction:column;
      align-items:center;
      justify-content:center;
      height:100vh;
      text-align:center;
      overflow:hidden;
    }
    h1{font-size:2.5rem;margin-bottom:10px;color:#00f0ff}
    p{font-size:1.1rem;margin-bottom:20px;color:#b6c2ff}
    .btn{
      background:linear-gradient(90deg,#00f0ff,#0044ff);
      padding:10px 20px;
      border:none;
      border-radius:8px;
      color:#fff;
      cursor:pointer;
      transition:0.3s;
    }
    .btn:hover{opacity:0.8;transform:scale(1.05)}
    .lang{
      position:fixed;
      top:10px;
      right:10px;
      background:#111;
      border-radius:20px;
      padding:5px 10px;
      font-size:14px;
    }
    .stars{
      position:absolute;
      width:100%;
      height:100%;
      background:url('https://i.ibb.co/mGzxK3Q/stars-bg.gif') center/cover;
      z-index:-1;
      opacity:0.6;
    }
  </style>
</head>
<body>
  <div class="stars"></div>
  <div class="lang">
    🌍 <button class="btn" id="langToggle">English</button>
  </div>

  <h1>بسم الله الرحمن الرحيم</h1>
  <h2>Cherrak Infinity ♾️</h2>
  <p>المنصة العالمية المتطورة — نظام يعتمد على الذكاء الاصطناعي والأقمار الصناعية الذكية 🛰️</p>

  <p id="stats">12,858 مستخدم متصل — $126,819.178 أرباح المستخدمين — سرعة الشبكة 3.3G</p>

  <button class="btn" onclick="window.location.href='https://github.com/cherrakH90'">زيارة GitHub</button>

  <footer style="margin-top:30px;font-size:0.9rem;opacity:0.8;">
    © 2025 Cherrak Infinity ♾️ — جميع الحقوق محفوظة
  </footer>

  <script>
    const langBtn = document.getElementById('langToggle');
    let arabic = true;
    langBtn.onclick = () => {
      if(arabic){
        document.documentElement.lang = 'en';
        document.documentElement.dir = 'ltr';
        document.querySelector('h1').textContent = 'In the name of Allah, the Most Merciful, the Most Compassionate';
        document.querySelector('h2').textContent = 'Cherrak Infinity ♾️';
        document.querySelector('p').textContent = 'The global advanced platform powered by Artificial Intelligence and Smart Satellites 🛰️';
        document.getElementById('stats').textContent = '12,858 connected users — $126,819.178 user earnings — 3.3G network speed';
        langBtn.textContent = 'العربية';
        arabic = false;
      } else {
        document.documentElement.lang = 'ar';
        document.documentElement.dir = 'rtl';
        document.querySelector('h1').textContent = 'بسم الله الرحمن الرحيم';
        document.querySelector('h2').textContent = 'Cherrak Infinity ♾️';
        document.querySelector('p').textContent = 'المنصة العالمية المتطورة — نظام يعتمد على الذكاء الاصطناعي والأقمار الصناعية الذكية 🛰️';
        document.getElementById('stats').textContent = '12,858 مستخدم متصل — $126,819.178 أرباح المستخدمين — سرعة الشبكة 3.3G';
        langBtn.textContent = 'English';
        arabic = true;
      }
    };
  </script>
</body>
</html>

===========================
Python Packaging User Guide
===========================

.. meta::
   :description: The Python Packaging User Guide (PyPUG) is a collection of tutorials and guides for packaging Python software.
   :keywords: python, packaging, guide, tutorial

.. toctree::
   :maxdepth: 2
   :hidden:

   overview
   flow
   tutorials/index
   guides/index
   discussions/index
   specifications/index
   key_projects
   glossary
   support
   contribute
   news

Welcome to the *Python Packaging User Guide*, a collection of tutorials and
references to help you distribute and install Python packages with modern
tools.

This guide is maintained on `GitHub`_ by the :doc:`Python Packaging Authority <pypa:index>`. We
happily accept :doc:`contributions and feedback <contribute>`. 😊

.. _GitHub: https://github.com/pypa/packaging.python.org


Overview and Flow
=================

.. note::

   Building your understanding of Python packaging is a journey. Patience and
   continuous improvement are key to success. The overview and flow sections
   provide a starting point for understanding the Python packaging ecosystem.

The :doc:`overview` explains Python packaging
and its use when preparing and distributing projects.
This section helps you build understanding about selecting the tools and
processes that are most suitable for your use case.
It includes what packaging is, the problems that it solves, and
key considerations.

To get an overview of the workflow used to publish your code, see
:doc:`packaging flow <flow>`.

Tutorials
=========

Tutorials walk through the steps needed to complete a project for the first time.
Tutorials aim to help you succeed and provide a starting point for future
exploration.
The :doc:`tutorials/index` section includes:

* A :doc:`tutorial on installing packages <tutorials/installing-packages>`
* A :doc:`tutorial on managing application dependencies <tutorials/managing-dependencies>`
  in a version controlled project
* A :doc:`tutorial on packaging and distributing <tutorials/packaging-projects>`
  your project

Guides
======

Guides provide steps to perform a specific task. Guides are more focused on
users who are already familiar with Python packaging and are looking for
specific information.

The :doc:`guides/index` section provides "how to" instructions in three major
areas: package installation; building and distributing packages; miscellaneous
topics.

Explanations and Discussions
============================

The :doc:`discussions/index` section provides in-depth explanations and discussion
about topics, such as:

* :doc:`discussions/deploying-python-applications`
* :doc:`discussions/pip-vs-easy-install`

Reference
=========

* The :doc:`specifications/index` section for packaging interoperability specifications.
* The list of :doc:`other projects <key_projects>` maintained by members of the Python Packaging Authority.
* The :doc:`glossary` for definitions of terms used in Python packaging.
