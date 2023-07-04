- 👋 Hi, I’m Charles Vosloo      github profile: journeyman33 email: voslooc@gmail.com
- 👀 I’m interested in DevOps and kubernetes
- 🌱 I have recently completed kubernetes certfications CKA and CKS.
- 🌱 I am persuing the Kodekloud Devops challenge presently Senior Devops Engineer status
- 💞️ I have collaborated on aws projects.

<!---
journeyman33/journeyman33 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

<!--START_SECTION:activity-->
name: Update README

on:
  schedule:
    - cron: '*/30 * * * *'
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    name: Update this repo's README with recent activity

    steps:
      - uses: actions/checkout@v2
      - uses: journeyman33/github-activity-readme@master
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

<!--END_SECTION:activity-->
