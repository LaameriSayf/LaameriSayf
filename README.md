<h1 align="center">👋 Hi, I’m <a href="https://github.com/LaameriSayf">Sayf Laameri</a></h1>

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=24&pause=1000&color=00BFFF&width=450&lines=Full-Stack+Developer;React+%7C+Spring+Boot+%7C+Node.js;Open+Source+Enthusiast;Lifelong+Learner" alt="Typing SVG" />
</p>

---

## 🚀 About Me

- 🔭 I’m currently working on cool full-stack projects  
- 🌱 I’m learning Kubernetes & AI tools  
- 💬 Ask me about Java, React, Node.js, Tailwind CSS  
- 📫 How to reach me: laamerisayf@gmail.com  
- ⚡ Fun fact: I love automating my daily tasks with bots 🤖  

---

## 🛠️ Tech Stack

<p align="center">
  <img alt="Java" src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
  <img alt="Spring Boot" src="https://img.shields.io/badge/SpringBoot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white" />
  <img alt="Node.js" src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white" />
  <img alt="Express.js" src="https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white" />
  <img alt="React" src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img alt="Tailwind CSS" src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" />
  <img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img alt="MySQL" src="https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white" />
</p>

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=LaameriSayf&show_icons=true&theme=radical" alt="GitHub stats" width="49%" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=LaameriSayf&theme=radical" alt="GitHub streak" width="49%" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=LaameriSayf&layout=compact&theme=radical" alt="Top Languages" />
</p>

---

## 🐍 GitHub Contribution Snake

<p align="center">
  <img src="https://github.com/LaameriSayf/LaameriSayf/blob/output/github-contribution-grid-snake.svg" alt="GitHub contribution snake" />
</p>

> **How to get the snake animation working:**  
> You need to add a GitHub Action workflow in your repository that generates this SVG automatically.  
> See the setup below!

---

## 🎯 How to enable the snake animation on your profile

Create a `.github/workflows/snake.yml` file in your repo with this content:

```yaml
name: Update GitHub Contribution Snake

on:
  schedule:
    - cron: '0 0 * * *'  # Runs every day at midnight UTC
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - uses: actions/checkout@v3

      - name: Generate contribution snake SVG
        uses: platane/snk@v1.6.4
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}

      - name: Commit & push
        run: |
          git config --local user.email "action@github.com"
          git config --local user.name "GitHub Action"
          git add github-contribution-grid-snake.svg
          git commit -m "Update contribution snake"
          git push
