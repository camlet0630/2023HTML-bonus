# 2023_HTML_bonus_track

# 待改的部分...
- [ ] 每次都跟當前 Agent 複述他上一次講了什麼，因為使用 API 的情況下每次都是獨立的，Agent 沒有記憶
- [ ] 每次提醒他們不要講太長
- [ ] 處理 .csv

# Related Link
+ github (bonus track 說明)：https://github.com/ariapoy/html.2023.bonusfinal-public
+ CRIT Evaluation: http://140.112.90.203:6271/
+ API reference: https://platform.openai.com/docs/api-reference/chat/create

# Files
1. HTML_chatUI_auto.ipynb: 可以自動使用 chatUI 的 ipynb 檔，下方有更詳細的說明
2. downloaded_file: 討論結束後下載的會議紀錄 (Export 功能)
3. `{name}.csv: 繳交至評分系統的 csv file`

# Warning!!
csv 的轉存極有可能出錯，請自行確認！  
（因為每次 agent 給出的格式並不相同）  
（當然，或許可以在要求他們給出最終答案時同時要求格式）

# HTML_chatUI_auto
## 執行完畢後...
+ 會下載一個 .txt，裡面紀錄了整場會議的內容
+ `很可能不可以上傳至評分系統的 .csv`

## 參數調整
+ **必須修改**
  - **Login**: teamname, passwrd 改成真正的
  - **設定主題**：name, subject_i 請改成這次要討論的主題
+ 其他可調整之處
  - config 請自行設定 (個人認為是先在同一主題下調整 config 以比較不同參數設定的差異) // n 似乎會關係到錢，請謹慎修改
  - **k: 辯論輪數**
  - 對話內容：目前完全參考助教給的對話 (自己加了 "當 B 不同意 A 統整的五個主題"、"當 A 或 B 有人還沒準備好" 時的處理方式)

## 消耗資源
if k=3
+ AI: 大約 $0.5 (即 0.08%)
+ time: 跑完一次大概要 40 分鐘


# Others
**tips:** 如果想用 py file，印象中可以上傳到 google colab，然後下載的時候選擇 .py
