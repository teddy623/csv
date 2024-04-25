# 基於 Diffie-Hellman 演算法的安全密鑰協商

這個範例演示了如何在量子計算環境下設計的密鑰協商算法，並結合了數字簽名或身份驗證以確保通信雙方的身份和訊息的完整性，從而提高演算法的安全性。

## 使用的套件

- cryptography：用於密鑰交換、數字簽名和密鑰派生
- os：用於生成隨機 AES 金鑰

## 如何安裝套件

首先，確保您已安裝了 Python。然後，使用以下命令安裝 cryptography 庫：

pip install cryptography

## 如何執行

python secure_key_exchange.py

## 執行結果

當您執行該程式時，您將看到以下輸出：
Signature verification successful.


這表示數字簽名已成功驗證，並且通信是安全的。

這個程式結合了 ECDH 進行密鑰交換，並使用 HKDF 技術來更新和派生密鑰，提供了更強的抗量子計算攻擊能力。同時，使用數字簽名對消息進行簽名和驗證，確保了消息的完整性，並防止了中間人攻擊。




