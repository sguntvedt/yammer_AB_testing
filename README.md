# yammer_AB_testing
### Contents
This repository contains two Juptyer notebooks that outline my approach to the "Validating A/B Test Results" challenge hosted by Mode Analytics. The first notebook constructs a database from four csv files in the datasets/yammer repository using the python's sqlite3 library. The second notebook queries this database to investigate the initial results of whether an update caused an increase user activity. Visualizations that aid this investigation are available in the enclosed Tableau packaged workbook.

### Description of CSV Files
1. "datasets/yammer/YAMMER_EMAILS.csv": This table contains events specific to the sending of emails.
2. "datasets/yammer/YAMMER_EVENTS.csv": This table includes one row per event, where an event is an action that a user has taken on Yammer. These events include login events, messaging events, search events, events logged as users progress through a signup funnel, events around received emails.
3. "datasets/yammer/YAMMER_EVENTS.csv": This table includes one row per user, with descriptive information about that user's account.
4. "datasets/yammer/YAMMER_EXPERIMENTS.csv": This table shows which groups users are sorted into for experiments. There should be one row per user, per experiment (a user should not be in both the test and control groups in a given experiment).

### Libraries
1. For Database Creation: sqlite3
2. Standard Data Science Libraries: numpy, pandas, scipy
3. For Visualizations: matplotlib, seaborn, Tableau Desktop
