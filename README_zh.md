
[English version 英文版](README.md)

# 廣告效益提升方案：A/B測試與機器學習實踐

## 專案概述
本專案透過A/B測試與機器學習模型，分析不同廣告策略對用戶轉化率的影響，旨在為企業提供基於數據驅動的廣告優化策略。

## 專案結構
- `數據探索性分析`：利用Pandas進行原始數據的處理與分析，NumPy進行數據的計算，從而識別轉化率影響因素。
- `A/B測試`：透過設計與實施A/B測試來評估廣告策略的有效性，並利用統計學方法驗證結果的顯著性。
- `模型建立與評估`：使用Scikit-learn建立隨機森林預測模型，並通過SMOTE技術解決樣本不平衡問題，提高模型對少數類的預測能力。
- `模型應用`：將訓練好的模型應用於新數據集，進行實時預測，以指導未來的廣告策略調整。

## 使用技術與工具
- `Pandas` 和 `NumPy`：數據處理與分析。
- `Matplotlib` 和 `Seaborn`：數據可視化，幫助洞察數據分佈和關鍵趨勢。
- `Scikit-learn`：機器學習算法實現和模型評估。
- `SMOTE`：處理數據不平衡問題，增強模型對少數類的學習能力。

## 模型訓練：
```python
from sklearn.model_selection import train_test_split
from sklearn.ensemble import RandomForestClassifier

# 劃分訓練集和測試集
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.25)

# 模型建立
model = RandomForestClassifier()
model.fit(X_train, y_train)

# 模型評估
accuracy = model.score(X_test, y_test)
print(f'模型準確率：{accuracy}')
```

## 貢獻指南
歡迎對本專案做出貢獻，無論是透過提供反饋、修正錯誤或是添加新功能。

## 聯絡方式
如有任何問題或建議，請通過郵件 w81015@gmail.com 聯繫。
