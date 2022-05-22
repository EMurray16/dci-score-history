# dci-score-history

DCI scores from 2000 onwards

This repository contains compiled DCI scores, going back to 2000. Why 2000? It's the first season in which DCI had the 40-30-30 format of scoring with subcaptions that closely resemble those used today. That said, past years farther back than 2000 may be added to this repository over time.

This data comes from 2 sources. Each has their own file format:

- [fromthepressbox.com](https://fromthepressbox.com/dca-dcihistory), which is used to get all scores prior to 2014. 

- [dci.org](https://dci.org/scores), which is used to get all scores from 2014 and onwards. This site could be used for 2013 scores, but at last check fromthepressbox had more complete recap information. 

The `combined` folder contains a merged score file with detail from both datasets. 

The code used to scrape the data from each source is not yet publicly available, because it's a pile of python, Javascritpt, R, and Go code, depending on running Google Chrome in a headless state. Code may be made publicly available in the relevant folders in the future.

## Download the data

There are three ways to download the data. 

1. If you are a Github user, you can clone the repository. 

2. If you are not a Github user, you can download this by clicking on the green "Code" button near the top of the page, and select "Download ZIP".

3. The full combined dataset can be accessed in code without directly downloading or cloning the repository by sending an HTTP GET request to the following URL: [https://raw.githubusercontent.com/EMurray16/dci-score-history/main/combined/allScores_2000to2019.csv](https://raw.githubusercontent.com/EMurray16/dci-score-history/main/combined/allScores_2000to2019.csv)

# Support

This data is freely and publicly available under an MIT License. It will always be this way. But, if you use this data and want to support my work, please consider donating to the [Michigan Drum Corps Scholarship Fund](https://midrumcorpsfund.org). I am a cofounder and current CEO, and your support would mean a lot to me! 100% of your donation would go towards keeping drum corps affordable for Michigan students.

[Please click here to donate via PayPal](https://www.paypal.com/donate/?hosted_button_id=CMMVPS28BGS5A)!
