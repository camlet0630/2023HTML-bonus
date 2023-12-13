# 2023_HTML_bonus_track

**tips:** 如果想用 py file，印象中可以上傳到 google colab，然後下載的時候選擇 .py

# Files
1. HTML_chatUI_auto.ipynb: 可以自動使用 chatUI 的 ipynb 檔，下方有更詳細的說明
2. downloaded_file: 討論結束後下載的會議紀錄 (Export 功能)
3. {name}.csv: 繳交至評分系統的 csv file


# HTML_chatUI_auto
## 執行完畢後...
+ 會下載一個 .txt，裡面紀錄了整場會議的內容
+ 可以上傳至評分系統的 .csv

## 參數調整
+ **必須修改**
  - **Login**: teamname, passwrd 改成真正的
  - **設定主題**：name, subject_i 請改成這次要討論的主題
+ 其他可調整之處
  - config 請自行設定 (個人認為是先在同一主題下調整 config 以比較不同參數設定的差異) // n 會關係到錢，請謹慎修改
  - **k: 辯論輪數**
  - 對話內容：目前完全參考助教給的對話 (自己加了 "當 B 不同意 A 統整的五個主題"、"當 A 或 B 有人還沒準備好" 時的處理方式)

### 消耗資源
+ AI: 大約 $0.45 (即 0.07%)
+ time: 跑完一次大概要 1-2 小時(?
