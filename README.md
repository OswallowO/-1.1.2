交易程式1.1.2版本更新速報
1. 開始交易功能可以運作。
2. 在「開始交易」功能中，程式會先檢查原資料夾中的日K線數據是否存在，並且判斷是否需要再次獲取日K的數據，此一功能可以確保程式可以有正確的漲停價，也可以避免過多的api資源浪費。
3. 「開始交易」功能現在可以在任何時候執行，在開盤以外的時間可以用來偵錯。
4. 目前還不能在使用者介面自定義分析的範圍，只能ctrl + F全域搜尋「wait_minutes_range」和「hold_minutes_range」來修改。
5. 目前還不能修改相似度的靈敏度，需要暫時使用0.3的靈敏度。
6. 當「開始交易」功能正在監測中，可以藉由輸入"Q"來退回主選單。
7. 請注意要安裝以下環境： (1)目前只支援Python 3.10 (2)如果執行後會馬上報錯，請輸入以下指令： pip install fugle-marketdata fugle-realtime pandas PyYAML numpy openpyxl colorama tabulate websocket-client
