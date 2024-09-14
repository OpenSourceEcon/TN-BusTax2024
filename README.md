# Data and code for "What Business Tax Reforms would be Best for Tennessee?"
This repository contains the data and code for the analyses by [Richard W. Evans](https://sites.google.com/site/rickecon) (@rickecon) in the September 2024 article on Tennessee business tax reform as part of the article "[Tennessee Trends: The State of Tennessee’s Economy](https://www.beacontn.org/tennessee-trends-the-state-of-tennessees-economy/)," by Ron Shultis, Jason Edmonds, and [Richard W. Evans](https://sites.google.com/site/rickecon), Beacon Center of Tennessee (Sep. 12, 2024).

## How to run the code from these analyses in the cloud in your browser
We have created a [Google Colab notebook](https://colab.research.google.com/drive/1dDKVTEAm4drvNXgHpm617j-82X4xzxKh?usp=sharing) with code almost exactly the same as th code in the Jupyter Notebook [`TN_BusTax2024.ipynb`](TN_BusTax2024.ipynb) decribed in the next section. The [Google Colab notebook](hhttps://colab.research.google.com/drive/1dDKVTEAm4drvNXgHpm617j-82X4xzxKh?usp=sharing) has the advantage of using a distribution of Python and corresponding packages that run in the cloud on remote servers instead of on your local machine. This allows you to use the notebook from any kind of device with a browser. You can execute th code, see the results, and save output to a temporary cloud folder from which you can download anything you want to keep.

## How to run the Jupyter Notebook on your machine
This repository contains a Jupyter Notebook [`TN_BusTax2024.ipynb`](TN_BusTax2024.ipynb) that can be run locally on your own machine to replicate the analyses in the paper. You can also modify this notebook to use for other analyses you might want to experiment with. To run this notebook locally on your machine, do the following steps:
* Fork and clone (or download) the https://github.com/OpenSourceEcon/TN-BusTax2024 repository
* In your computer's terminal, navigate to the directory of the `TN-BusTax2024` repository on your local machine.
* Create the conda environment `tn-bustax2024-dev` by typing the following command: `conda env create -f environment.yml`
* Activate the `tn-bustax2024-dev` conda environment by typing the following command: `conda activate tn-bustax2024-dev`
* This should allow your notebook to run while this conda environment is activated.

## Files and directories in the repository
This repository contains the following items:
* [`TN_BusTax2024.ipynb` Jupyter notebook](TN_BusTax2024.ipynb). An executable notebook you can use to replicate all the analyses in the article and creation of output and figures. A corresponding [Google Colab notebook](https://colab.research.google.com/drive/1dDKVTEAm4drvNXgHpm617j-82X4xzxKh?usp=sharing) that can be run on your browser and executed in the cloud is available at the link in this sentence.
[`environment.yml`](environment.yml). Conda environment file for creating conda environment `tn_bustax2024-dev`.
* [`/data/` directory](data/). This directory contains the data used in the analyses in the article.
    * [`/data/Main202306.xlsx`](/data/Main202306.xlsx). Data for "Revenue Collections, Tennessee Department of Revenue, June 2023. PDF of report is [here](https://www.tn.gov/content/dam/tn/revenue/documents/pubs/2023/Coll202306.pdf). Data downloaded from [here](https://www.tn.gov/content/dam/tn/revenue/documents/statistics/2023/Main202306.xlsx).
    * [`/data/ReservesBalancesData.xlsx`](/data/ReservesBalancesData.xlsx). Rainy Day Fund and Total Reserves and Balances data for all 50 states and DC, Pew Charitable Trusts, Dec. 7, 2023. (Data downloaded from: https://www.pewtrusts.org/en/research-and-analysis/articles/2022/10/18/-/media/data-visualizations/interactives/2016/fiscal-50/docs/2013/reservesbalancesdata.xlsx?v=20231206)
    * [`/data/Tab3.xlsx`](/data/Tab3.xlsx). Data and calculations for Table 3 in the paper.
    * [`/data/fig4_source.csv`](/data/fig4_source.csv). Source data for Figure 4 in the paper.
    * [`/data/fig5_source.csv`](/data/fig5_source.csv). Source data for Figure 5 in the paper.
* [`/images/` directory](images/). This folder contains the `.html` files for the dynamic visualizations in the paper and created in the notebook and the corresponding static `.png` image files.
    * [`/images/fig4_tn_raintotbal_tseries.html`](/images/fig4_tn_raintotbal_tseries.html). Dynamic data visualization Bokeh `.html` file. Figure 4. Tennessee Rainy Day fund and total reserves as a percentage of general fund expenditures: 2000-2023.
    * [`/images/fig4_tn_raintotbal_tseries.png`](/images/fig4_tn_raintotbal_tseries.png). Static `.png` file. Figure 4. Tennessee Rainy Day fund and total reserves as a percentage of general fund expenditures: 2000-2023.
    * [`/images/fig5_rain_totbal_pct_2023.html`](/images/fig5_rain_totbal_pct_2023.html). Dynamic data visualization Bokeh `.html` file, for web publication. Figure 5. State 2023 Rainy day Fund Balances and Total Fund Balances as Percent of General Fund Expenditures.
    * [`/images/fig5_rain_totbal_pct_2023.png`](/images/fig5_rain_totbal_pct_2023.png). Static `.png` file, for web publication. Figure 5. State 2023 Rainy day Fund Balances and Total Fund Balances as Percent of General Fund Expenditures.
