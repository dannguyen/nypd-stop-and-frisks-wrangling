# Downloading the files


https://www1.nyc.gov/site/nypd/stats/reports-analysis/stopfrisk.page


```sh
mkdir -p downloaded 

cd downloaded

curl -O https://www1.nyc.gov/assets/nypd/downloads/zip/analysis_and_planning/stop-question-frisk/sqf-200[3-9]-csv.zip

curl -O https://www1.nyc.gov/assets/nypd/downloads/zip/analysis_and_planning/stop-question-frisk/sqf-201[1-4]-csv.zip

curl -O https://www1.nyc.gov/assets/nypd/downloads/excel/analysis_and_planning/stop-question-frisk/sqf-201[5-6].csv

curl -o sqf-2017.xlsx \
    https://www1.nyc.gov/assets/nypd/downloads/excel/analysis_and_planning/stop-question-frisk/csi-2947-2019-sqf-cy2017-updated1-9-2020.xlsx

curl -O https://www1.nyc.gov/assets/nypd/downloads/excel/analysis_and_planning/stop-question-frisk/sqf-201[8-9].xlsx

```
