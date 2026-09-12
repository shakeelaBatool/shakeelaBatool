<div align="center">

  <!-- Blue Waving Banner -->
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:00203F,100:0077B6&height=200&section=header&text=Shakeela%20Batool&fontSize=40&fontColor=ffffff&subtext=AI/ML%20Enthusiast%20%C2%B7%20Data%20Science%20Learner&subFontSize=18&subColor=ADE8F4" width="100%" />
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&pause=1000&color=0088FF&center=true&vCenter=true&width=700&lines=AI+%26+Machine+Learning+Enthusiast;Data+Science+Learner" alt="Typing SVG" />
  </a>

</div>


## 🔍 What I'm Passionate About
- 📊 **Data Science** – Turning data into meaningful insights  
- 💻 **Programming** – Writing clean and efficient Python code  
- 📈 **Machine Learning** – Exploring algorithms that make systems smarter  
- 🌐 **Education** – Empowering girls through modern education  

---

## 🌟 Featured Projects
- 🧠 **Conditional Probability Project**
- 💱 **Currency Converter (Python)**
- 🔢 **Prime Number Finder**
- 🎮 **Hangman Game**

---

name: GitHub Analytics

on:
  # Update analytics automatically every day
  schedule:
    - cron: "0 0 * * *"

  # Allow you to run it manually
  workflow_dispatch:

jobs:
  github-analytics:

    runs-on: ubuntu-latest

    permissions:
      contents: write

    steps:

      - name: Generate GitHub Analytics
        uses: lowlighter/metrics@latest

        with:

          # ==================================================
          # YOUR GITHUB USERNAME
          # ==================================================

          user: shakeelaBatool

          # GitHub token
          token: ${{ secrets.METRICS_TOKEN }}

          # Name of generated analytics file
          filename: github-analytics.svg

          # Pakistan timezone
          config_timezone: Asia/Karachi

          # Large dashboard
          config_display: large


          # ==================================================
          # BASIC PROFILE INFORMATION
          # ==================================================

          base: header, activity, community, repositories, metadata


          # ==================================================
          # ISOMETRIC CONTRIBUTION CALENDAR
          # ==================================================

          plugin_isocalendar: yes

          plugin_isocalendar_duration: full-year


          # ==================================================
          # MOST USED LANGUAGES
          # ==================================================

          plugin_languages: yes

          plugin_languages_limit: 12

          plugin_languages_details: bytes-size, percentage

          plugin_languages_sections: most-used, recently-used


          # ==================================================
          # CODING HABITS
          # ==================================================

          plugin_habits: yes

          plugin_habits_facts: yes

          plugin_habits_charts: yes

          plugin_habits_days: 14


          # ==================================================
          # CONTRIBUTION CALENDAR
          # ==================================================

          plugin_calendar: yes

          plugin_calendar_limit: 1


          # ==================================================
          # ACHIEVEMENTS
          # ==================================================

          plugin_achievements: yes

          plugin_achievements_display: compact


          # ==================================================
          # RECENT ACTIVITY
          # ==================================================

          plugin_activity: yes

          plugin_activity_limit: 5

          plugin_activity_days: 30


          # ==================================================
          # ERROR HANDLING
          # ==================================================

          plugins_errors_fatal: no




