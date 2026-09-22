# Stephen Curry season dashboard

Open index.html in your browser. Internet access is needed to load D3.
The three charts show 3P%, points per game, and eFG% from the supplied CSV.
Career totals are excluded. The 2019-20 season includes only 5 games.
Data is embedded in index.html; editing curry.csv alone does not update the charts.

## Publish
Copy these files into your local repository, then commit and push:

    git add index.html curry.csv README.md
    git commit -m "Add Curry season dashboard"
    git push -u origin main

In your GitHub repository, open Settings > Pages.
Choose Deploy from a branch, main, / (root), then Save.
When deployment finishes, the expected URL is:
https://johnbang-hs.github.io/steph-curry-is-he-playing-well/
