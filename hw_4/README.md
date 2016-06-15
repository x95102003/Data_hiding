#Hw_4
##Trellis code and linear correlation

###需求:  


###遭遇困難

1. 隱藏message128後再分析上都會找出不正確的其他路徑。  
2. 分佈沒有依照 gauss unit variance 在尋找路徑上會有些微影響。
3. 從圖片取出來的pixel並沒有屬於gauss分佈，若用該vector會找不到正確路徑。

###解決方式

1. 取高斯數值的時候做round，減少後面取整產生比較大的誤差，可以準確找出128
2. 調整gauss參數，符合standard gauss即可。
3. 需要扣掉向量平均。


###實驗結果
![Analysis Result](./linear_correlation.png)