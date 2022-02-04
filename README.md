- 👋 Hi, I’m @arduan
- 👀 I’m interested in ...
- 🌱 I’m currently learning Python, HTML, CSS, SQL, Flask, Django, JavaScript
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
arduan/arduan is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
[![Ashutosh's github activity graph](https://activity-graph.herokuapp.com/graph?username=arduan)](https://github.com/ashutosh00710/github-readme-activity-graph)
![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=arduan&theme=solarized_dark)

Статистика языков в коммитах:
![](https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=arduan&theme=solarized_dark)

Статистика языков в репозиториях:
![](https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=arduan&theme=solarized_dark)

Статистика профиля:
![](https://github-profile-summary-cards.vercel.app/api/cards/stats?username=arduan&theme=solarized_dark)

Данные по коммитам за сутки:
![](https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=arduan&theme=solarized_dark)

name: Waka Readme

on:
  schedule:
    # Runs at 12am IST
    - cron: '30 18 * * *'
  workflow_dispatch:
jobs:
  update-readme:
    name: Update Readme with Metrics
    runs-on: ubuntu-latest
    steps:
      - uses: anmol098/waka-readme-stats@master
        with:
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
          GH_TOKEN: ${{ secrets.GH_TOKEN }}
