# Downloading the files


https://www1.nyc.gov/site/nypd/stats/reports-analysis/stopfrisk.page


```sh
mkdir -p downloaded 

cd downloaded

## 2003-9.csv
curl -O https://www1.nyc.gov/assets/nypd/downloads/zip/analysis_and_planning/stop-question-frisk/sqf-200[3-9]-csv.zip
## 2010-14.csv
curl -O https://www1.nyc.gov/assets/nypd/downloads/zip/analysis_and_planning/stop-question-frisk/sqf-201[0-4]-csv.zip

## 2015.csv 2016.csv
curl -o 2015.csv https://www1.nyc.gov/assets/nypd/downloads/excel/analysis_and_planning/stop-question-frisk/sqf-2015.csv

curl -o 2016.csv https://www1.nyc.gov/assets/nypd/downloads/excel/analysis_and_planning/stop-question-frisk/sqf-2016.csv

curl -o sqf-2017.xlsx \
    https://www1.nyc.gov/assets/nypd/downloads/excel/analysis_and_planning/stop-question-frisk/csi-2947-2019-sqf-cy2017-updated1-9-2020.xlsx

curl -O https://www1.nyc.gov/assets/nypd/downloads/excel/analysis_and_planning/stop-question-frisk/sqf-201[8-9].xlsx

```

## Converting to csv

```sh
in2csv sqf-2017.xlsx | rg '\(null\)' -r '' --passthru > 2017.csv
in2csv sqf-2018.xlsx | rg '\(null\)' -r '' --passthru > 2018.csv
in2csv sqf-2019.xlsx | rg '\(null\)' -r '' --passthru > 2019.csv
```
