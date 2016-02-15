Example-Neural-Network-MLP Document
=========

程式執行說明
-----------------------

此次作業實作 MLP ，除了設定 選擇檔案、學習率、學習次數 欄位之類，加上了 新增隱藏層 的功能，每按一下”新增隱藏層”就會多一層隱藏層，接著輸入欄位來設定該隱藏層的神經元個數。另外此次也將執行按鈕分成 “訓練”和“測驗” 兩個按鈕。

在界面上，最左邊欄加上了 console output 的 Panel ，將來會顯示部分執行過程中的 RMSE 和正確率。

程式簡介和實驗結果
-----------------------

程式使用多層感知機的架構，並藉由倒傳遞演算法來修正鍵節值，而由於架構包含隱藏層，比起單層感知機，對於非線性的數值運算和判斷有較好的表現。實際去跑 IRIS , wine, breast-cancer-wisconsin, 579 四個資料集，結果如下：

### IRIS ###

![IRIS.png](http://imgur.com/qA3JSON.png)

### wine ###

![wine.png](http://imgur.com/5bUOmLJ.png)

### 579 ###

![579.png](http://imgur.com/47DVKdR.png)

### breast-cancer-wisconsin ###

![breast-cancer-wisconsin.png](http://imgur.com/IGfI67W.png)

### XOR ###

![XOR.png](http://imgur.com/Pc2N79b.png)

實驗結果分析與討論
-----------------------

實際去跑資料集時，發現並不是越多隱藏層，正確率就會越好，相反的，有時隱藏層越多，正確率反而越低，個人認為隱藏層的神經元數目以及相關鍵節值反倒是影響正確率比較多，其中牽扯倒傳遞演算法和鍵節值的變化量是否有加入慣性項等，可惜這次沒有實作到慣性項而無法確實比較。
