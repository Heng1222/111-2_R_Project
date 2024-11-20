# 111-2_R_Project 逐時氣象&空氣指標分析與預測

**動機**


近年來，氣候變遷以及工業科技發展對全球氣溫、降水量和空氣品質造成不穩定的影響，氣候異常和空氣不良也成為大眾日常討論的議題。其中，PM2.5對人體健康的危害極大，氣溫變化也大大影響各行各業的日常。本專案旨在透過R語言進行資料整理建立分析模型，以預測未來的氣溫變化和PM2.5含量，也同時探討影響降水量的因素。

**分析方法**

本專案以Python進行網頁爬蟲，並以R語言進行主要分析製作

**目的**

以2022年的實際資料為基礎，利用迴歸分析模型、ANOVA檢定、AIC檢定以及邏輯斯迴歸等方式進行建模。同時，利用2020年和2021年的歷史資料作測試，來驗證模型的預測力。
我們以四個問題進行探討：

問題一：我們對資料集進行基本統計觀測，了解資料分布情況和資料彼此間的關係

問題二：我們針對PM2.5含量進行建模預測，探討PM2.5含量受哪些因素影響並且建立模型預測未來PM2.5含量

問題三：針對氣溫變化進行建模預測，探討氣溫變化受到哪些因素的影響，也同時建立模型預測未來氣溫走勢

問題四：對是否降雨進行檢定預測，探討降雨量受哪些因素的影響

藉由歷史資料分析和建模，預測未來氣候變化和PM2.5含量趨勢。透過這次專案結果可以為政府和大眾提供一些參考依據，未來若須制定更有效的環保政策或設施時可以參考。

**資料來源與整理**


使用資料集以下兩個資料集為原始資料，並進行資料整理與轉置後合併
1.<行政院環境保護署-空氣品質歷年監測資料> https://airtw.epa.gov.tw/CHT/Query/His_Data.aspx
2.<中央氣象局-觀測資料查詢> https://e-service.cwb.gov.tw/HistoryDataQuery/index.jsp

**檔案**
`downloadData.py` - 下載每日觀測資料

`GenerateCSV.py` -  將下載的csv檔合併

`main.R` - 主要執行檔


**使用套件**
Python：
```
selenium
pandas
glob
```

R：
```
lubridate
ggplot2
GGally
reshape2
scales
coefplot
```
