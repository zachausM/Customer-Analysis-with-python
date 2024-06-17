## Customer analysis project

### Instructions on how to set up python on your computer
1. Download a free version of anaconda from this link https://www.anaconda.com/download
2. Open jupyter Notebook
3. Start running your python codes

### Data analysis Using Python
1. Installation of various python packages
   
     import matplotlib.pyplot as plt
   
     import pandas as pd'
   
     from sklearn.cluster import KMeans
   
     from sklearn.processing import StandardScaler
   
     from sklearn.datasets import make_blobs
   
     from sklearn.metrics import silhouette_score
   
     import seaborn as sns
   
3. Loading data to jupyter notebook
   
    file_path = r'C:/Users/pc/OneDrive/Documents/Mall_Customers.csv'
   
    df = pd.read_csv(file_path)
   
5. Showing the customer data
   
    print(df.head())

7. Plotting a histogram
   
   plt.figure(figsize = (14, 6))
   
   plt.subplot(1, 3, 1)
   
   sns.histplot(df['Age'], kde=True, bins=20)
   
   plt.title('Age Distribution')
