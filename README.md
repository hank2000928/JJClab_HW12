# JJClab_HW12
VM虛擬機裝載Virtual Nano Lab License

## Step 1. 檢查 209 主機

確認主機系統與License Server 程式，並查看網路監聽。

<img width="946" height="815" alt="image" src="https://github.com/user-attachments/assets/f275f704-854f-4ac7-bd69-f22dddcc2bec" />

## Step 2. 檢查VMware 虛擬機

確認 VM 識別資訊，確認 VM 網卡與路由，查詢前往 209 的路由即測試連通性。

<img width="883" height="312" alt="image" src="https://github.com/user-attachments/assets/46558a62-4ae3-4849-84a4-f5bcd01769c2" />
<img width="867" height="523" alt="image" src="https://github.com/user-attachments/assets/8e0120b1-5b98-4d5b-85eb-0e200d9b37ef" />
<img width="833" height="470" alt="image" src="https://github.com/user-attachments/assets/400524eb-1394-497d-aa07-d56876f70113" />
<img width="842" height="258" alt="image" src="https://github.com/user-attachments/assets/5e999529-1bac-4673-b3e7-47cd953955b6" />

因設置固定IP，預計裝載於sle15-b。

## Step 3. LM-X 授權環境盤點

從執行中的程序確認 LM-X 位置，查看 LM-X 工作目錄後，確認授權服務仍在運作。

<img width="950" height="356" alt="image" src="https://github.com/user-attachments/assets/82108de0-965c-4aa0-8b0e-ec67f0ecf304" />
<img width="936" height="464" alt="image" src="https://github.com/user-attachments/assets/9f74fc31-a6b3-4396-97a5-8de80a965512" />

確認209 主機安裝的是 LM-X 4.8.1 系列工具，而且目錄中有三份不同名稱的 License 檔案。
目前執行中的 LM-X 使用的 License 路徑，與安裝目錄中的 License 路徑不同。

<img width="945" height="155" alt="image" src="https://github.com/user-attachments/assets/e6545f17-9c44-4f3b-af19-5e2983333192" />
<img width="931" height="552" alt="image" src="https://github.com/user-attachments/assets/93252c0d-6b11-4ad1-87f5-be2d4ee79816" />
<img width="947" height="552" alt="image" src="https://github.com/user-attachments/assets/ae598632-4be1-4eb4-be84-0854aec33bd9" />

確認 209 的 HostID 類型

<img width="936" height="596" alt="image" src="https://github.com/user-attachments/assets/7d443fc8-837a-44af-bc28-aa5aee8bfc9a" />

## Step 4. 確認 VM 的程式相容性

從 sle15-b 測試 SFTP 與一般檔案傳輸

<img width="839" height="266" alt="image" src="https://github.com/user-attachments/assets/fb9668c9-90c5-4c1b-980f-9d93d16deaef" />
<img width="836" height="269" alt="image" src="https://github.com/user-attachments/assets/52c73ba9-bba3-4ba7-9c92-14a2ccea5f64" />

核對 LM-X 安裝程式的平台需求。

<img width="835" height="270" alt="image" src="https://github.com/user-attachments/assets/8c529a1d-9391-4016-b38d-092209055b10" />

確認 209 的 LM-X 執行檔相容性

<img width="952" height="312" alt="image" src="https://github.com/user-attachments/assets/a3093e40-d545-446e-8c11-8e7b84ffb6ce" />

檢查 sle15-b 的函式庫環境

<img width="938" height="240" alt="image" src="https://github.com/user-attachments/assets/3709a021-47f1-46dd-a971-b07e1d715a06" />
<img width="841" height="128" alt="image" src="https://github.com/user-attachments/assets/f5c196ee-0995-4a35-84eb-4303b7104ad8" />
<img width="838" height="309" alt="image" src="https://github.com/user-attachments/assets/2fe67e4e-268b-40c8-b235-d3da62d1d91f" />

準備 LM-X 程式副本

<img width="832" height="185" alt="image" src="https://github.com/user-attachments/assets/ec26ab72-1541-409c-99f4-8d806e01e535" />
<img width="933" height="226" alt="image" src="https://github.com/user-attachments/assets/a0bf1229-e5c9-436f-9354-2b8be514ea60" />
<img width="848" height="465" alt="image" src="https://github.com/user-attachments/assets/eb0aa547-c607-4d69-b3c2-8e74925e288f" />
<img width="953" height="166" alt="image" src="https://github.com/user-attachments/assets/9cb5c8b1-6f81-4e5a-b906-1a03482c9158" />
<img width="831" height="122" alt="image" src="https://github.com/user-attachments/assets/6450f888-80c6-4be0-ac22-db36c7ad5a4f" />


## Step 5. VM建立獨立 License Server

<img width="844" height="218" alt="image" src="https://github.com/user-attachments/assets/32bbc9c2-2fe2-4c2e-b48e-de2e4a2a10c0" />

在 sle15-b 建立專用設定檔

<img width="840" height="323" alt="image" src="https://github.com/user-attachments/assets/514a6b01-f58c-4c68-a4a0-9fdd4a2d6e12" />

建立測試授權目錄

<img width="831" height="575" alt="image" src="https://github.com/user-attachments/assets/fd8a215e-f0e5-4a85-bf89-e1db1b9415e2" />

啟動 LM-X License Server

<img width="846" height="724" alt="image" src="https://github.com/user-attachments/assets/de1fe8b0-da72-4f23-b95c-f09a7e9a10eb" />

從 sle15-a 測試新 Server

<img width="837" height="115" alt="image" src="https://github.com/user-attachments/assets/32bc1c44-1540-454a-9b40-dd21a5852253" />
<img width="877" height="57" alt="image" src="https://github.com/user-attachments/assets/46f2eccd-64ba-41e5-aa3c-19733f4bde65" />
<img width="837" height="432" alt="image" src="https://github.com/user-attachments/assets/97e195dc-d1e1-4cb9-aa6b-050a42bced16" />
