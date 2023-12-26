<div align="center">
<h1>
  MacroTrends Scraper
  </h1>
  <a href="https://www.macrotrends.net/">
  <img src="https://i.imgur.com/j6tEOJG.png" width="200">
  </a>
  </div>
  

# EN-US
## About
Scraping and managing data for US Stocks from MacroTrends

[Repository](https://github.com/capuccino26/Finance)

## Pre-Requisites
The script uses Chrome as the webdriver, you need to have chromedriver.exe in the path, you can download the lastest version from [ChromeDriver][https://github.com/mozilla/geckodriver/releases](https://chromedriver.chromium.org/downloads)

## How-to
* User insert the tickers separated by comma when asked and send;
* The following messages will show accordingly:
  * SUCCESS: When the ticker was found in MacroTrends database and the data were successfully scraped.
  * EMPTY TICKER: When the ticker was found in MacroTrends database but there is no data available.
  * INVALID TICKER: When the ticker was not found in MacroTrends database.
* For the successfully scraped data the program will create a new folder called STOCKUS/TICKER under Path for each inserted ticker.
* The folder contains a table with the raw data obtained and a figure with plots of important data.

# PT-BR
## Sobre
Raspagem e manipulação de dados para ações americanas utilizando o site MacroTrends

[Repositório](https://github.com/capuccino26/Finance)

## Pré-requisitos
O código utiliza o Chrome como webdriver, será necessário o arquivo geckodriver.exe no Path, é recomendado o download da versão mais recente: [ChromeDriver]([https://github.com/mozilla/geckodriver/releases](https://chromedriver.chromium.org/downloads))

## Utilização
* O usuário insere os tickers separados por vírgula e inicia o programa;
* As seguintes mensagens serão exibidas de acordo:
  * SUCCESS: Quando o ticker foi encontrado na database do Macrotrends e os dados foram extraídos com sucesso.
  * EMPTY TICKER: Quando o ticker foi encontrado na database do Macrotrends mas não existem dados disponíveis.
  * INVALID TICKER: Quando o ticker não foi encontrado na database do MacroTrends.
* Para os dados extraídos com sucesso o programa irá gerar uma nova pasta em Path chamada "STOCKUS/TICKER" para cada ticker inserido.
* A pasta contém a tabela com todos os dados brutos e uma figura com os principais dados obtidos.

# Example
  * User inserts: OCN,OCSL,OFED,OFG,OFS,OFSSH
  * Output shows:
  ```
  OCN
SUCCESS
OCSL
SUCCESS
OFED
SUCCESS
OFG
SUCCESS
OFS
SUCCESS
OFSSH
INVALID TICKER
  ```
  * Resulting main folder:
  
  ![alt text](https://i.imgur.com/wNec6uN.png)
  
  * Resulting ticker folder:
  
  ![alt text](https://i.imgur.com/M2exU2C.png)
  
  * Resulting graphs image:
  
  ![alt text](https://i.imgur.com/1vmdavT.png)
  
  * Data in the excel file:
```
Dates
Revenue
Cost Of Goods Sold
Gross Profit
Research And Development Expenses
SG&A Expenses
Other Operating Income Or Expenses
Operating Expenses
Operating Income
Total Non-Operating Income/Expense
Pre-Tax Income
Income Taxes
Income After Taxes
Other Income
Income From Continuous Operations
Income From Discontinued Operations
Net Income
EBITDA
EBIT
Basic Shares Outstanding
Shares Outstanding
Basic EPS
EPS - Earnings Per Share
Cash On Hand
Receivables
Inventory
Pre-Paid Expenses
Other Current Assets
Total Current Assets
Property Plant And Equipment
Long-Term Investments
Goodwill And Intangible Assets
Other Long-Term Assets
Total Long-Term Assets
Total Assets
Total Current Liabilities
Long Term Debt
Other Non-Current Liabilities
Total Long Term Liabilities
Total Liabilities
Common Stock Net
Retained Earnings (Accumulated Deficit)
Comprehensive Income
Other Share Holders Equity
Share Holder Equity
Total Liabilities And Share Holders Equity
Net Income/Loss
Total Depreciation And Amortization - Cash Flow
Other Non-Cash Items
Total Non-Cash Items
Change In Accounts Receivable
Change In Inventories
Change In Accounts Payable
Change In Assets/Liabilities
Total Change In Assets/Liabilities
Cash Flow From Operating Activities
Net Change In Property Plant And Equipment
Net Change In Intangible Assets
Net Acquisitions/Divestitures
Net Change In Short-term Investments
Net Change In Long-Term Investments
Net Change In Investments - Total
Investing Activities - Other
Cash Flow From Investing Activities
Net Long-Term Debt
Net Current Debt
Debt Issuance/Retirement Net - Total
Net Common Equity Issued/Repurchased
Net Total Equity Issued/Repurchased
Total Common And Preferred Stock Dividends Paid
Financial Activities - Other
Cash Flow From Financial Activities
Net Cash Flow
Stock-Based Compensation
Common Stock Dividends Paid
Current Ratio
Long-term Debt / Capital
Debt/Equity Ratio
Gross Margin
Operating Margin
EBIT Margin
EBITDA Margin
Pre-Tax Profit Margin
Net Profit Margin
Asset Turnover
Inventory Turnover Ratio
Receiveable Turnover
Days Sales In Receivables
ROE - Return On Equity
Return On Tangible Equity
ROA - Return On Assets
ROI - Return On Investment
Book Value Per Share
Operating Cash Flow Per Share
Free Cash Flow Per Share
```
