<!-- Header -->
<h1 align="center">Hi, I'm **Kushagra** 👋</h1>
<p align="center">Wasting life away </p>

---


<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=k-u-s-h-a-g-r-a-k-e-d-i-a&show_icons=true&theme=tokyonight&hide_border=true" alt="GitHub stats" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=k-u-s-h-a-g-r-a-k-e-d-i-a&theme=tokyo-night" alt="Activity graph" />
</p>

---

### 🔥 GitHub Streak
<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=k-u-s-h-a-g-r-a-k-e-d-i-a&theme=tokyonight&utcOffset=5.5" alt="Productive time" />
</p>



### 💻 Tech Stack
<p align="center">
  <img src="https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white" alt="C" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/SQL-003B57?style=for-the-badge&logo=mysql&logoColor=white" alt="SQL" />
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML" />
</p>

---

<!-- Optional snake / contribution image -->
<p align="center">
  name: Generate Snake

on:
  workflow_dispatch:
  schedule:
    - cron: "0 0 * * *"

permissions:
  contents: write

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Generate snake
        uses: Platane/snk@v3
        with:
          github_user_name: k-u-s-h-a-g-r-a-k-e-d-i-a
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark

      - name: Push to output branch
        uses: crazy-max/ghaction-github-pages@v3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
</p>
