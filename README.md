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
          TODOIST_API_KEY: ${{c1ef8408ed19ed548887e7de2dd227b6b44ea0d9}}
          PREMIUM: ""
<!-- TODO-IST:END -->
