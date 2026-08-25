<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0F1729,100:36BCF7&height=200&section=header&text=Mamoon%20Siddiqui&fontSize=42&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Computer%20Science%20Engineer%20%C2%B7%20Full-Stack%20Developer&descAlignY=58&descSize=16&descColor=9BAFD9" width="100%" alt="banner" />

</div>

## 01 · About

| | |
|---|---|
| 🔭 **Currently** | Building full-stack apps + competitive programming |
| 🌱 **Learning** | Advanced React patterns, system design, DSA optimization |
| 💼 **Open to** | Full-time roles and collaborative projects |
| 🎯 **Goal** | Contributing to open-source, shipping impactful software |

> *"Coding is just a piece of cake with a sprinkle of venom!"* ⚡🍰

## 02 · Stack

<div align="center">

**Languages**
<br>
<img src="https://skillicons.dev/icons?i=py,js,java,cpp,c,dart,php" />

**Frontend**
<br>
<img src="https://skillicons.dev/icons?i=html,css,react,flutter" />

**Backend**
<br>
<img src="https://skillicons.dev/icons?i=nodejs,express,flask,django" />

**Database & Cloud**
<br>
<img src="https://skillicons.dev/icons?i=mysql,postgres,mongodb,sqlite,firebase" />

**Tools**
<br>
<img src="https://skillicons.dev/icons?i=git,github,figma,tensorflow" />

</div>

## 03 · GitHub stats

**What was actually broken, and the real fix:**

| Widget | Old status | Root cause |
|---|---|---|
| Streak stats | ❌ Dead | `github-readme-streak-stats.herokuapp.com` — Heroku killed free dynos in 2022, domain will never come back |
| Stats + top langs | ⚠️ Flaky | Shared public Vercel instance shares one GitHub API quota across *everyone* using it — hits the 5k req/hr limit and drops for all users at once |
| Trophies | ⚠️ Flaky | Same shared-instance rate-limit problem |
| Activity graph | ⚠️ Flaky | Same shared-instance rate-limit problem |

Swapping domains doesn't fix the flaky ones — any shared public instance will hit the same wall eventually. The maintainers' own recommendation is to stop depending on a live fetch entirely: use the **[github-readme-stats-generator](https://github.com/marketplace/actions/github-readme-stats-generator)** GitHub Action, which runs on a schedule (e.g. daily via cron) and commits static SVGs straight into your profile repo. A static file in your repo can't be rate-limited or go down.

**Setup (one-time, ~5 min):**

1. In your `Mamoon-5G/Mamoon-5G` profile repo, add `.github/workflows/stats.yml`:

```yaml
name: Update GitHub stats
on:
  schedule:
    - cron: '0 0 * * *'   # daily at midnight UTC
  workflow_dispatch:
jobs:
  update-stats:
    runs-on: ubuntu-latest
    permissions:
      contents: write
    steps:
      - uses: jstrieb/github-stats@master
        with:
          username: Mamoon-5G
          exclude_repos:
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

2. The action commits `generated/overview.svg` and `generated/languages.svg` to your repo.
3. Embed them as normal images:

```md
![Stats](./generated/overview.svg)
![Top Languages](./generated/languages.svg)
```

Until that's wired up, the cards below still point at the public instances (fine most of the time, just not bulletproof):

<div align="center">
  <img width="48%" src="https://github-readme-stats.vercel.app/api?username=Mamoon-5G&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" />
  <img width="48%" src="https://streak-stats.demolab.com/?user=Mamoon-5G&theme=tokyonight&hide_border=true" />
</div>

<div align="center">
  <img width="60%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Mamoon-5G&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" />
</div>

<div align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=Mamoon-5G&theme=tokyonight&no-frame=true&no-bg=true&margin-w=4&row=1&column=6" />
</div>

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Mamoon-5G&theme=tokyo-night&hide_border=true&bg_color=0D1117&color=7C3AED&line=7C3AED&point=FFFFFF" />
</div>

## 04 · Connect

| Platform | Handle |
|---|---|
| 💼 LinkedIn | [mamoon-siddiqui](https://www.linkedin.com/in/mamoon-siddiqui-0a27b2296/) |
| 🐙 GitHub | [Mamoon-5G](https://github.com/Mamoon-5G) |
| 🐦 X / Twitter | [@Mamoon_4G](https://x.com/Mamoon_4G) |
| 📸 Instagram | [@m_a__siddiqui_5g_](https://www.instagram.com/m_a__siddiqui_5g_) |
| 👥 Facebook | [mamoon.siddiqui.146](https://www.facebook.com/mamoon.siddiqui.146) |
| 🧩 LeetCode | [Mamoon-5G](https://leetcode.com/u/Mamoon-5G/) |
| ♟️ Lichess | [MAMOON_4G](https://lichess.org/@/MAMOON_4G) |
| ✉️ Email | siddiquimamoon2004ms@gmail.com |

<br>

<div align="center">

<img src="https://komarev.com/ghpvc/?username=Mamoon-5G&style=flat-square&color=7C3AED" alt="Profile Views" />

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:36BCF7,100:0F1729&height=130&section=footer" width="100%" />

<em>"Code is poetry written in logic, and every bug is just a plot twist waiting to be resolved."</em> ✨
<br><br>
**Thanks for visiting — star a repo if you find it useful!**

</div>
