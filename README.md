- š Hi, Iām @Mokenadoa
- š Iām interested in ...
- š± Iām currently learning ...
- šļø Iām looking to collaborate on ...
- š« How to reach me ...

<!---
Mokenadoa/Mokenadoa is a āØ special āØ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
name: GitHub Actions Demo
run-name: ${{ github.actor }} is testing out GitHub Actions š
on: [push]
jobs:
  Explore-GitHub-Actions:
    runs-on: ubuntu-latest
    steps:
      - run: echo "š The job was automatically triggered by a ${{ github.event_name }} event."
      - run: echo "š§ This job is now running on a ${{ runner.os }} server hosted by GitHub!"
      - run: echo "š The name of your branch is ${{ github.ref }} and your repository is ${{ github.repository }}."
      - name: Check out repository code
        uses: actions/checkout@v3
      - run: echo "š” The ${{ github.repository }} repository has been cloned to the runner."
      - run: echo "š„ļø The workflow is now ready to test your code on the runner."
      - name: List files in the repository
        run: |
          ls ${{ github.workspace }}
      - run: echo "š This job's status is ${{ job.status }}."
