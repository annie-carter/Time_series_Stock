# Stock Anaylsis 
# <bu>Time Series Project</bu>
* by Annie Carter, MSN, BS, RN
* Sourced by Yahoo Finance
  
![Image-3.png](https://images.theconversation.com/files/526640/original/file-20230516-23-zv2vps.jpg?ixlib=rb-1.1.0&rect=121%2C80%2C4372%2C2910&q=20&auto=format&w=320&fit=clip&dpr=2&usm=12&cs=strip)

## <u>Background</u>
Apple (AAPL), Microsoft (MSFT), Visa (V), and American Express (AXP) are four prominent and influential companies in their respective industries. Apple, founded in 1976, is an innovative technology giant known for its groundbreaking products like the iPhone and Mac computers. Microsoft, established in 1975, is a software and cloud computing powerhouse, recognized for its Windows operating system and Office suite of applications. Visa, founded in 1958, is a global leader in electronic payment solutions, facilitating secure transactions and digital payments worldwide. American Express, dating back to 1850, is a well-established financial services company known for its premium credit cards and extensive rewards programs. These companies have consistently displayed robust financial performance, brand loyalty, and widespread global impact, making them attractive options for investors seeking stability and diverse investment opportunities in the stock market.

## <u>Project Description</u>
This Time-Series Machine Learning project is focused on forecasting future stock prices for four prominent companies: Apple Inc. (AAPL), Microsoft Corporation (MSFT), Visa Inc. (V), and American Express Company (AXP). Leveraging historical stock price data and pertinent financial indicators, the project aims to create precise predictive models capable of analyzing and projecting stock price fluctuations over time. The project will utilize comprehensive historical stock price datasets for AAPL, MSFT, V, and AXP, incorporating factors such as trading volumes, market trends, and relevant macroeconomic data. Employing advanced Time-Series ML algorithms, the project strives to offer valuable insights into potential upcoming stock price trends for these industry leaders. Accurate stock price predictions for these esteemed companies can play a pivotal role for investors, enabling informed decisions and the identification of lucrative investment prospects. The project's outcomes hold the potential to guide investors and financial experts in formulating effective trading strategies and optimizing investment portfolios based on dependable future stock price forecasts.

## <u>Project Goal</u>

The primary objective of this project is to construct a robust Time-Series Machine Learning forecasting model that utilizes historical stock price data, market indicators, and pertinent financial variables for Apple Inc. (AAPL), Microsoft Corporation (MSFT), Visa Inc. (V), and American Express Company (AXP). By employing advanced Time-Series ML algorithms, the project endeavors to accurately forecast future stock price movements for these distinguished companies. The forecasting model will be developed to offer insightful predictions regarding potential trends and fluctuations in stock prices, furnishing investors and financial experts with well-informed insights to enhance decision-making and optimize their investment approaches. The accomplishment of this project will contribute to heightened financial planning, risk mitigation, and investment decision-making for stakeholders engaged with these industry-leading entities.


## <u>Initial Questions</u>
1. Can ML time series analysis accurately predict the future stock prices of Apple Inc. (AAPL), Microsoft Corporation (MSFT), Visa Inc. (V), and American Express Company (AXP) based on historical stock price data and relevant market indicators?

2. How well can ML time series models identify trends and patterns in the historical stock price data of AAPL, MSFT, V, and AXP, assisting investors in making informed decisions about potential stock price movements?

3. Can ML time series forecasting unveil any seasonality or cyclical patterns in the stock prices of AAPL, MSFT, V, and AXP, offering valuable insights for traders and investors to fine-tune their strategies?



## <u>Data Dictionary</u>
The initial dataset comprised of three dataframes, 7 columns, which expanded to 8 columns after preparation. It contained 1758 rows. Date column used as indexed and converted to datetime data type. Column "Symbol" added to sort different stock symbols.  

|   Target         |       Datatype           |                Definition                   |
|:----------------:|:------------------------:|:-------------------------------------------:|
|   Close          |       float64            |The opening price of the stock for that day.


|  Attribute       |       Datatype           |                Definition                   |
|:----------------:|:------------------------:|:-------------------------------------------:|
|Date              | 5028 non-null  int64     | The date of the trading day.         |
|Open              | 5028 non-null  object | The opening price of the stock for that day.          |
|High              | 5028 non-null  object |The highest price the stock reached during that day.              |    
|Low  | 5028 non-null  object |  The lowest price the stock reached during that day.   |
|Dividend | 5028 non-null  object | Any dividends paid out on that day.        |
|Stock Split        | 537407 non-null  object | Any stock splits that occurred on that day.|
|Symbol | 5028 non-null  object | Stock Symbol of company      |


## <u>Statistical Testing Hypothesis </u>
Autoregressive Integrated Moving Average (ARIMA) and SARIMAX (Seasonal AutoRegressive Integrated Moving Average with eXogenous regressors) Modeling: 
## <u>Planning Process</u>
#### Planning
1. Clearly define the problem statement related to Yahoo Finance Stock market dataset for Apple, Microsoft, Visa and American Express company, including essential information for addressing the chronic disease of interest.

2. Create a detailed README.md file documenting the project's context, dataset characteristics, and analysis procedure for easy reproducibility.

#### Acquisition and Preparation
3. Preprocess the data, handling missing values and outliers effectively during data loading and cleansing.

4. Perform feature selection meticulously, identifying influential features impacting the prevalence of the chronic disease through correlation analysis, feature importance estimation, or domain expertise-based selection criteria.

5. Develop specialized scripts (e.g., wrangle.py or acquire.py and prepare.py) for efficient and consistent data acquisition, preparation, and data splitting.

6. Safeguard proprietary aspects of the project by implementing confidentiality and data security measures, using .gitignore to exclude sensitive information.

#### Exploratory Analysis
7. Utilize exploratory data analysis techniques, employing compelling visualizations and relevant statistical tests to extract meaningful patterns and relationships within the dataset.

#### Modeling
8. Carefully choose a suitable machine learning algorithm, evaluating options like Moving Averages (MA),  Autoregressive Integrated Moving Average (ARIMA), SARIMAX time-series analysis task.

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
2. Before proceeding, ensure that you have the necessary database credentials. Get data set from https://finance.yahoo.com/quote/ stock symbol historic data for five years 
Create .gitignore for privacy if necessary
3. Clone the classification_project repository from my GitHub or download the following files: aquire.py, wrange.py or prepare.py, and final_report.ipynb. You can find these files in the project repository.
4. Open the final_report.ipynb notebook in your preferred Jupyter Notebook environment or any compatible Python environment.
5. Ensure that all necessary libraries or dependent programs are installed. You may need to install additional packages if they are not already present in your environment.
6. Run the final_report.ipynb notebook to execute the project code and generate the results.
By following these instructions, you will be able to reproduce the analysis and review the project's final report. Feel free to explore the code, visualizations, and conclusions presented in the notebook.


## <u>Key Findings</u>
### ** AAPL findings = 
    
## <u>Conclusion</u>

## <u>Next Steps</u>


## <u>Recommendations</u>   
    
## <u>References</u>
Dhaduk, H. (2021, July 18). Stock market forecasting using Time Series analysis With ARIMA model.

