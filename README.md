# "Shut it down!" A detention data dashboard

[![Coverage Status](https://coveralls.io/repos/github/detentiondatadashboard/detention-data-dashboard/badge.svg?branch=main)](https://coveralls.io/github/detentiondatadashboard/detention-data-dashboard?branch=main)

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Software Dependencies](#software-dependencies)
- [Directory Structure](#directory-structure)
- [Design and Technology Review](#design-and-technology-review)
- [Demos](#demos)
- [Limitations](#limitations)
- [References](#references)


### Project Overview

This collaborative project is an extension of work by the Center for Human Rights (CHR)  at the University of Washington. Through numerous FOIA requests and litigation, CHR obtained dozens of datasets spanning roughly 2010-2020 related to Immigration and Customs Enforcement (ICE) migrant detention facilities across the US. These datasets tracked variables related to detention facilities, law enforcement, and bond rates. This project created an interactive dashboard and downloadable package for public consumption to make the data more widely available and assist with holding ICE accountable for its detention policies. 

This project included developing an interaction design, technology review, and robust testing to ensure accuracy. In our team of three, I was personally responsible for the geographic analysis of the data (mapping used in the dashboard), developing the testing of the final output, and creating a package that could be pip installed in Python. This project served as the final project for CSE 583: Software Development for Data Scientists. This repo is a clone of the original repo, and the dashboard and package are no longer maintained due to prohibitive costs. However, video demos of the final product are available below in the “results” section.


### Data Sources

All data courtesy of the University of Washington's Center for Human Rights. These datasets were painstaking obtained through numerous FOIA requests and litigation. Datasets span roughly 2010-2020 and are related to Immigration and Customs Enforcement (ICE) migrant detention facilities across the US. Datasets are divided between tracking encounters with immigration enforcement, arrests, removals, and ICE facilities. Due to the large size of the datasets, we temporarily paid for Git Large File Storage (LFS)  to host the data online. Furthermore, analysis was complicated due to ICE not providing coding tables for their datasets. Consequently, secondary literature and expert interviews were frequently required to decipher the meaning of particular columns and coding used in these datasets.

The head of a typical dataset looks similar to the following:
<img width="1174" alt="Screenshot 2023-11-22 at 3 42 12 PM" src="https://github.com/lucaskolson/ICE_Detention_Data_Dashboard/assets/91341415/2aa72d83-8ecb-47c1-b8c2-5fac6202a819">


### Software Dependencies

- Python3
- For required python packages, see requirements.txt


### Directory Structure

```bash
.
├── LICENSE
├── Procfile
├── README.md
├── app.py
├── data
│   ├── README.md
│   ├── arrest_dtypes.yaml
│   ├── arrests.csv
│   ├── arrests_by_fy.csv
│   ├── encounter_dtypes.yaml
│   ├── encounters.csv
│   ├── ice-facilities.csv
│   ├── removal_dtypes.yaml
│   └── removals.csv
├── detention_data_dashboard
│   ├── __init__.py
│   └── tests
│       ├── __init__.py
│       └── test_core.py
├── doc
│   ├── Tech\ Review\ -\ Web\ Development\ Apps\ for\ Python.txt
│   ├── Technology\ Review\ -\ Dashboards\ in\ Python.pptx
│   └── software_design.md
├── environment.yml
├── plot_downloads
│   └── test.png
├── requirements.txt
└── runtime.txt
```

### Design and Technology Review

![Interaction Diagram](https://github.com/lucaskolson/ICE_Detention_Data_Dashboard/assets/91341415/39c69f72-c9ac-48cb-be8b-94d90bb39b40)

<img width="960" alt="Screenshot 2023-11-22 at 3 49 26 PM" src="https://github.com/lucaskolson/ICE_Detention_Data_Dashboard/assets/91341415/5c801478-8e4d-4bb4-b52e-4f0b4cabaf59">


### Demos

Demos of the final dashboard and pip installed package are available in the videos below. Due to prohibitive costs, the dashboard and package are not actively maintained.

[![Dashboard Demo](https://img.youtube.com/vi/6wihXwGH7GE/0.jpg)](https://www.youtube.com/watch?v=6wihXwGH7GE)
[![Dashboard Demo](https://img.youtube.com/vi/fuL_vFVhTDs/0.jpg)](https://www.youtube.com/watch?v=fuL_vFVhTDs)


### Limitations

The largest limitations of this project are both the size and messiness of the original datasets. Hosting all the datasets on GitHub required paying for Git LFS, and we did not continue this payment beyond the period of our class project. Additionally, the datasets lacked coding so we spent a considerable amount of time deciphering the meaning of codes to create a useful analysis. 


### References

UW Center for Human Rights, https://jsis.washington.edu/humanrights/
