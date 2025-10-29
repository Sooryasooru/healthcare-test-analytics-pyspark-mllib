Healthcare Test-Analytics Dashboard
Real-time | PySpark MLlib | 5-sec refresh | Password tunnel

 What it does?
Upload your healthcare CSV → get a live dashboard that
refreshes every 5 seconds
trains MLlib models (regression, classification, clustering)
exposes a public URL with password protection

 30-Second Start (Google Colab)?
Open the notebook:
](https://colab.research.google.com/drive/1-0YxqxV4AiNHS-acTHs6FDuPZQcHdXmI)Upload your CSV → run the single cell

Click the URL printed at the end
Enter password: soorya123
That’s it – fully live dashboard in half a minute.

 Screens
KPI cards (Tests, Patients, Hospitals, Abnormal %, ML Accuracy)
Monthly & Quarterly trends (live lines/bars)
Hospital performance (drill-down)
Doctor workload vs abnormal-rate (bubble)
City distribution (treemap)
Confusion matrix & heat-maps
All charts move every 5 seconds.


ML Models
Table
Copy
Model	Target	Metric
Random-Forest Regression	ResultValue	RMSE ↓ live
Random-Forest Classification	AbnormalResult	Accuracy ↑ live
K-Means Clustering	Patient segments	Silhouette ↑ live


🔧 Customise
Password → change in notebook cell 6
Refresh rate → change REFRESH = 5000 (ms)
Columns → edit cat_cols / num_cols in cell 5


 Repo Structure
Copy
healthcare-test-analytics-pyspark-mllib/
├── healthcare_dashboard.ipynb   # single Colab notebook
├── README.md                    # this file
├── export/                      # auto-generated charts + CSV
├── streamlit_app.py             # auto-generated dashboard code
└── requirements.txt             # pip list
🛑 Stop
Restart runtime or run the “Stop switch” cell in the notebook.
📄 Licence
MIT – do whatever you want with it.
Made with ❤️ by Soorya
