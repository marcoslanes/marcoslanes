![visitors](https://visitor-badge.glitch.me/badge?page_id=page.id&left_color=green&right_color=red)

<!-- TODO-IST:START -->
name: Todoist Readme

on:
  workflow_dispatch:
  schedule:
    # Runs every minute
    - cron: "* * * * *"

jobs:
  update-readme:
    name: Update todoist stats
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: abhisheknaiidu/todoist-readme@master
        with:
          TODOIST_API_KEY: ${{ secrets.TODOIST_API_KEY }}
          PREMIUM: ""
<!-- TODO-IST:END -->
