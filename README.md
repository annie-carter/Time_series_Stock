# Stock Anaylsis 
# <bu>Time Series Project</bu>
* by Annie Carter
* Sourced by Yahoo Finance
![Image-3.png](https://images.theconversation.com/files/526640/original/file-20230516-23-zv2vps.jpg?ixlib=rb-1.1.0&rect=121%2C80%2C4372%2C2910&q=20&auto=format&w=320&fit=clip&dpr=2&usm=12&cs=strip)

## <u>Background</u>
Coca-Cola, Nike, and Boeing are three prominent and well-established companies with a rich history in their respective industries. Coca-Cola, founded in 1886, is an iconic beverage company known for its signature carbonated soft drink that has become a global symbol of refreshment and happiness. Nike, established in 1964, is a renowned sportswear and athletic footwear manufacturer, recognized for its cutting-edge designs and extensive endorsement of world-class athletes. Boeing, founded in 1916, is a leading aerospace company that has played a pivotal role in shaping the aviation industry with its innovative aircraft, including commercial airliners, defense systems, and space exploration technologies. Over the years, these companies have demonstrated strong financial performance, brand loyalty, and global market presence, making them sought-after choices for investors seeking stable and diverse investment opportunities in the stock market.

## <u>Project Description</u>
This Time-Series Machine Learning project aims to forecast future stock prices for three prominent companies: The Coca-Cola Company (KO), Nike Inc. (NKE), and The Boeing Company (BA). Utilizing historical stock price data and other relevant financial indicators, this project seeks to develop accurate predictive models that can analyze and predict stock price movements over time. The comprehensive historical stock price datasets for KO, NKE, and BA will be utilized, along with factors like trading volumes, market trends, and relevant macroeconomic data. By applying advanced Time-Series ML algorithms, this project aims to provide valuable insights into potential future stock price trends for these companies. Accurate stock price predictions for these industry leaders can be instrumental for investors in making informed decisions and identifying investment opportunities. The project's results have the potential to guide investors and financial professionals in developing effective trading strategies and optimizing investment portfolios based on reliable future stock price forecasts.

## <u>Project Goal</u>

The primary goal of this project is to develop a robust Time-Series Machine Learning forecasting model that leverages historical stock price data, market indicators, and relevant financial factors for The Boeing Company (BA), The Coca-Cola Company (KO), and Nike Inc. (NKE). By applying advanced Time-Series ML algorithms, the project aims to accurately predict future stock price movements for these prominent companies. The forecasting model will be designed to provide valuable insights into potential trends and fluctuations in stock prices, aiding investors and financial professionals in making well-informed decisions and optimizing their investment strategies. The project's success will contribute to improved financial planning, risk management, and investment decision-making for stakeholders interested in these industry-leading companies


## <u>Initial Questions</u>
1. Can ML time series analysis accurately predict the future stock prices of The Coca-Cola Company (KO), Nike Inc. (NKE), and The Boeing Company (BA) based on historical stock price data and relevant market indicators?

2. How well can ML time series models identify trends and patterns in the historical stock price data of KO, NKE, and BA, helping investors make informed decisions about potential stock price movements?

3. Can ML time series forecasting reveal any seasonality or cyclical patterns in the stock prices of KO, NKE, and BA, providing valuable insights for traders and investors to adjust their strategies accordingly?

4. Is there any correlation between external factors such as economic indicators, news sentiment, or industry-specific events, and the time series forecast of stock prices for KO, NKE, and BA, offering a deeper understanding of the stock market behavior for these companies?

## <u>Initial Questions</u>
The initial dataset comprised of three dataframes, 7 columns, which expanded to 8 columns after preparation. It contained 1758 rows. Date column used as indexed and converted to datetime data type. Column "Symbol" added to sort different stock symbols.  

|   Target         |       Datatype           |                Definition                   |
|:----------------:|:------------------------:|:-------------------------------------------:|
|   Close          |       float64            |The opening price of the stock for that day.


|  Attribute       |       Datatype           |                Definition                   |
|:----------------:|:------------------------:|:-------------------------------------------:|
|Date              | 1758 non-null  int64     | The date of the trading day.         |
|Open         | 1758 non-null  object | The opening price of the stock for that day.          |
|High  | 1758 non-null  object |The highest price the stock reached during that day.              |    
|Low  | 1758 non-null  object |  The lowest price the stock reached during that day.   |
|Dividend | 1758 non-null  object | Any dividends paid out on that day.        |
|Stock Split        | 537407 non-null  object | Any stock splits that occurred on that day.|
|Symbol | 1758 non-null  object | Stock Symbol of company      |


## <u>Statistical Testing Hypothesis </u>
Autoregressive Integrated Moving Average (ARIMA) Modeling: 
## <u>Planning Process</u>
#### Planning
1. Clearly define the problem statement related to Yahoo Finance Stock market dataset for Boeing, Nike, Coca-Cola company, including essential information for addressing the chronic disease of interest.

2. Create a detailed README.md file documenting the project's context, dataset characteristics, and analysis procedure for easy reproducibility.

#### Acquisition and Preparation
3. Preprocess the data, handling missing values and outliers effectively during data loading and cleansing.

4. Perform feature selection meticulously, identifying influential features impacting the prevalence of the chronic disease through correlation analysis, feature importance estimation, or domain expertise-based selection criteria.

5. Develop specialized scripts (e.g., wrangle.py or acquire.py and prepare.py) for efficient and consistent data acquisition, preparation, and data splitting.

6. Safeguard proprietary aspects of the project by implementing confidentiality and data security measures, using .gitignore to exclude sensitive information.

#### Exploratory Analysis
7. Utilize exploratory data analysis techniques, employing compelling visualizations and relevant statistical tests to extract meaningful patterns and relationships within the dataset.

#### Modeling
8. Carefully choose a suitable machine learning algorithm, evaluating options like Moving Averages (MA), Holt's Linear Exponential Smoothing, Autoregressive Integrated Moving Average (ARIMA),  time-series analysis task.

9. Implement the selected machine learning models using robust libraries (e.g., scikit-learn, statsmodel), systematically evaluating multiple  time series models models (MA, Holt's Linear Trend, ARIMA)
10. Train the models rigorously to ensure optimal learning and model performance.

11. Conduct rigorous model validation techniques to assess model generalization capability and reliability.

12. Select the most effective model, such as ARIMA or HLT, based on thorough evaluation metrics for further analysis.

#### Product Delivery
13. Assemble a final notebook, combining superior visualizations, well-trained models, and pertinent data to present comprehensive insights and conclusions with scientific rigor.

14. Generate a Prediction.csv file containing predictions from the chosen model on test data for further evaluation and utilization.

15. Maintain meticulous project documentation, adhering to scientific and professional standards, to ensure successful presentation or seamless deployment.

## <u>Instructions to Reproduce the Final Project Notebook</u> 
To successfully run/reproduce the final project notebook, please follow these steps:

1. Read this README.md document to familiarize yourself with the project details and key findings.
2. Before proceeding, ensure that you have the necessary database credentials. Get data set from https://finance.yahoo.com/quote/BA/history?p=BA
, https://finance.yahoo.com/quote/KO?p=KO&.tsrc=fin-srch, https://finance.yahoo.com/quote/NKE/history?p=NKE
Create .gitignore for privacy if necessary
3. Clone the classification_project repository from my GitHub or download the following files: aquire.py, wrange.py or prepare.py, and final_report.ipynb. You can find these files in the project repository.
4. Open the final_report.ipynb notebook in your preferred Jupyter Notebook environment or any compatible Python environment.
5. Ensure that all necessary libraries or dependent programs are installed. You may need to install additional packages if they are not already present in your environment.
6. Run the final_report.ipynb notebook to execute the project code and generate the results.
By following these instructions, you will be able to reproduce the analysis and review the project's final report. Feel free to explore the code, visualizations, and conclusions presented in the notebook.


## <u>Key Findings</u>

    
## <u>Conclusion</u>

## <u>Next Steps</u>


## <u>Recommendations</u>   
    
## <u>References</u>
