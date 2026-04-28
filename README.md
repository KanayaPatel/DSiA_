# DSiA_
Project done in Rori Rolfs' DSCI410L (Data Science in Action) Course @ University of Oregon

After CAHOOTS was defunded in April 2025, the city of Eugene lost one of its organizations who would assist in a majority of welfare check calls. Most, if not all welfare check calls are now in the hands of the EPD. Given this, prior members of CAHOOTS asked us to take a look into the gaps the defunding caused. Specifically for this project, how have welfare checks been handled
(by EPD? MCSLC?). Has Welfare Check call volume changed? Has there beena change in the number of arrests during these welfare check calls?

Here is the structure of the project: 

DSiA/
└── data/
│   ├── 2015-2025 SPD Calls for Service.xlsx
│   ├── 2015-2025 SPD Responding Units.xlsx
│   ├── EugeneCAD2015noloc.csv                           
│   ├── EugeneCAD2016noloc.csv
│   ├── EugeneCAD2017noloc.csv
│   ├── EugeneCAD2018noloc.csv
│   ├── EugeneCAD2019noloc.csv
│   ├── EugeneCAD2020noloc.csv
│   ├── EugeneCAD2021noloc.csv
│   ├── EugeneCAD2022noloc.csv
│   ├── EugeneCAD2023noloc.csv
│   ├── EugeneCAD2024noloc.csv
│   ├── EugeneCAD2025noloc.csv
│   └── MCSLC.xlsx
├── cleaned_eug_c.csv
├── cleaned_eug_no_c.csv
├── cleaned_spd.csv
├── data.ipynb
└── requirements.txt

NOTE: The .csv files not being in the data folder is intentional. 

Here is the order in which files should be ran: 
1. Before running, ensure that Python 3.13 is installed on your device. After, open a powershell terminal and ensure you're in the DSiA directory. Then run the command: ```pip install -r "requirements.txt"```. This will download the packages required to run the files. 
2. Run the ```clean_data.ipynb```file
   a. This will provide the cleaned datasets that we see in the stucture: cleaned_eug_c.csv, cleaned_eug_no_c.csv, and cleaned_spd.csv.
3. Run the ```volume_analysis.ipynb``` file
   a. This will provide an image of a difference of differences plot named "diff_in_diff.png" which tells us how the volume of welfare check calls changed after CAHOOTS was defunded. This        will use Springfield as a control, as they still have their version of CAHOOTS.
   b. NOTE: This file is incomplete
5. Run the ```outcome_analysis.ipynb``` file
   a. This will provide an image of a KDE distribution plot which tells how the number of arrests made during welfare checks changed after CAHOOTS was disbanded.
   b. NOTE: This file is incomplete.

README will be updated as more files are created. 
