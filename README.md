# 美食評論語意分析

1. **資料匯入與初步觀察：**
   - 程式碼使用 `pandas` 庫匯入一個包含5,000筆資料的CSV檔案。
   - 使用 `head()` 函數顯示資料的前幾筆觀測值。

2. **使用 CountVectorizer 建立 Term Document Matrix：**
   - 利用 `CountVectorizer` 將文字資料轉換成詞頻矩陣（term document matrix）。
   - 顯示矩陣的形狀。

3. **移除無意義的字詞（Stop Words）：**
   - 使用 `CountVectorizer` 指定英文的停用詞（stop words）進行文字處理。
   - 再次顯示矩陣的形狀。

4. **進行降維：**
   - 使用 TruncatedSVD（奇異值分解的一種形式）進行降維，維度降至2維。
   - 展示降維後的數據形狀。
   - 繪製降維後的數據散點圖，分析文本在二維空間的分佈。

5. **繪製字詞分佈圖：**
   - 利用 TruncatedSVD 針對字詞進行降維。
   - 繪製字詞降維後的數據散點圖。

6. **進行 TF-IDF 分析：**
   - 使用 `TfidfVectorizer` 進行 TF-IDF（Term Frequency-Inverse Document Frequency）轉換。
   - 繪製 TF-IDF 降維後的數據散點圖。
   - 展示字詞的分佈。

7. **篩選特定主題的字詞：**
   - 透過數值篩選，找出在降維後的數據中特定主題上重要的字詞。
   - 顯示篩選結果，列出相應的字詞。

8. **結論：**
   - 最後，根據對降維後的數據的分析，得出一些文本評論傾向正向的結論。
