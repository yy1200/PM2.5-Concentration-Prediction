## Data Set Information
The datatime period is between Jan 1st, 2010 to Dec 31st, 2014. Missing data are denoted as -1.

### Attribute Information

- No: row number
- year: year of data in this row
- month: month of data in this row
- day: day of data in this row
- hour: hour of data in this row
- pm2.5: PM2.5 concentration (ug/m^3)
- DEWP: Dew Point 
- TEMP: Temperature
- PRES: Pressure (hPa)
- cbwd: Combined wind direction
- Iws: Cumulated wind speed (m/s)
- Is: Cumulated hours of snow
- Ir: Cumulated hours of rain

## 步驟
1. Data preprocessing
2. MINMAXSCALER
3. 時間序列資料的特徵轉換
4. 建 MODEL (LSTM)

## Result
Test **RMSE** = 3.26559；Test **MAE** = 1.94512 
![image](https://github.com/yy1200/PM2.5-Concentration-Prediction/assets/92247082/b70d73b7-e087-447e-b403-6a13f7cf295d)

## Comparison
- LGBMREGRESSOR

  **RMSE** = 4.1423；**MAE** = 2.2537
  ![image](https://github.com/yy1200/PM2.5-Concentration-Prediction/assets/92247082/40a6b129-eec2-4dd7-89a9-6146401c108d)
- GRADIENTBOOSTINGREGRESSOR

  **RMSE** = 4.4083；**MAE** = 2.3426
  ![image](https://github.com/yy1200/PM2.5-Concentration-Prediction/assets/92247082/11eaaba6-866e-49b6-8e6e-025b85a22dfe)
- XGBOOST

  **RMSE** = 5.3502；**MAE** = 2.6947
  ![image](https://github.com/yy1200/PM2.5-Concentration-Prediction/assets/92247082/2eee97e1-fbb2-4200-8117-13f8ffa8fa08)



