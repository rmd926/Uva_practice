# 🔢 GPE 10605 - Count the Trees
![image](https://github.com/user-attachments/assets/27f969a1-968e-4b46-832d-dc539fe7f68c)

## 題目敘述

給定 n 個不同元素，求使用這些元素可構成的不同標記二元樹的數量。  
例如，當 n=1 時，只有一棵樹；當 n=2 時，有四種不同的標記二元樹。

---

## 解題提示（Hint）

- 此問題即為計算第 n 個 Catalan 數。  
- Catalan 數公式為：  
![image](https://github.com/user-attachments/assets/feb8339a-8768-4be5-a5bc-afcc90091afb)



- 可使用動態規劃從 C_0 開始遞推到 C_n。  
- 輸入多組 n，輸出對應的 Catalan 數。

---

## 解題流程說明

1. 計算階乘  
   - 預先計算 0 到 MAX（此處為 600）階乘值，儲存在 fact 陣列中，避免重複計算。

2. 讀取輸入  
   - 持續讀取整數 n，直到讀到 0 終止。

3. 計算 Catalan 數（計算不同標記二元樹數量）  
   - 使用公式：  
     ![image](https://github.com/user-attachments/assets/d0e90125-5cd9-498f-bf55-5a09ef71c830)
 
   - 利用事先計算好的階乘值快速計算。

4. 輸出結果  
   - 輸出計算得到的 C_n。

---

此作法利用組合數公式直接計算 Catalan 數，比動態規劃更有效率且簡潔。
