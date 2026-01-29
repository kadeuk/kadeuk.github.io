---
layout: single
title: "Home"
author_profile: true
---

# 👨‍💻 Kadeuk의 기술 블로그

안녕하세요!  
**"늦었다고 생각할 때가 진짜 시작이다"** 83년생, **M365 관리자**와 **운영 엔지니어**를 꿈꾸는 **Kadeuk**입니다.

## 🎯 학습 목표
1. **Microsoft 365** 완벽 이해 (MS-900, MD-102)
2. **Windows Server & Network** 기초 다지기
3. **매일 꾸준히** 기록 남기기

---
### 📝 최신 글

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span style="font-size:small; color:gray;">({{ post.date | date: "%Y-%m-%d" }})</span>
    </li>
  {% endfor %}
</ul>