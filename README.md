# iKaros Monitoring and Analytics for Social Media
iKaros 輿情分析系統
透過socketio與server溝通


## How to use?

```python
python SM2socketio.py
```

```python
node /testserver/index001.js
```

```python
python /web/bbb.py
```
## socketio
    self.socketio.on('801', self.getkeywords)
    self.socketio.on('802', self.ptt_Crawler)
    self.socketio.on('803', self.showfilename)
    self.socketio.on('804', self.CrawlerFlag)
    self.socketio.on('805', self.get_news)
    self.socketio.on('806', self.get_google)


## SM2socketio.py
```
nutc-dslde-MBP:sm2-master nutc_dsl$ python SM2sockitio.py
connect
handshake2 002
801
getkeywords [{"name": "柯文哲", "contents": ["用藍綠分析去看柯，好像看不出所以然，一下子說兩岸一家親，", "柯P 說當然", "人尷尬的話語，他在對岸說兩岸一家親其實我覺得沒甚麼關係，"]}, {"name": "選情", "contents": ["柯P 說當然", "藍營鐵票在60～70萬上下，由此可見民進黨不跑票柯一定落選", "滿意度7成卻因為藍綠問題而無法連任的狀況類似，柯很可能因為民進黨"]}, {"name": "臺北", "contents": ["臺北市溫泉發展協會今年特別開發一支專為臺北溫泉季打造的APPIn向北投，下載APP", "讓民眾瞭解溫泉文化的魅力與特色，臺北市政府觀光傳播局每年協助北投溫泉業者舉辦觀", "第17屆臺北溫泉季11月1日至5日在北投地區盛大登場，今年溫泉季以名湯海灣宴潑湯祈"]}, {"name": "現以", "contents": ["北部人發現以前吃的都是南部粽時在想什麼", "我某朋友是個霸凌者", "分享一個我國中隔壁班轉學生的故事"]}, {"name": "參賽", "contents": ["若全民同意 > 走申請程序 > 中華奧會變更為臺灣奧會 > 參賽", "若全民同意 > 走申請程序 > 中華奧會變更為臺灣奧會 > 參賽", "上過國際談判桌的人都知道，這種重大的事件，中間要跑的流程很多"]}]
```

## index001.js

```
nonutc-dslde-MBP:testserver nutc_dsl$ node index001.js
001
401
801
getkeywords:  [{"name": "柯文哲", "contents": ["用藍綠分析去看柯，好像看不出所以然，一下子說兩岸一家親，", "柯P 說當然", "人尷尬的話語，他在對岸說兩岸一家親其實我覺得沒甚麼關係，"]}, {"name": "選情", "contents": ["柯P 說當然", "藍營鐵票在60～70萬上下，由此可見民進黨不跑票柯一定落選", "滿意度7成卻因為藍綠問題而無法連任的狀況類似，柯很可能因為民進黨"]}, {"name": "臺北", "contents": ["臺北市溫泉發展協會今年特別開發一支專為臺北溫泉季打造的APPIn向北投，下載APP", "讓民眾瞭解溫泉文化的魅力與特色，臺北市政府觀光傳播局每年協助北投溫泉業者舉辦觀", "第17屆臺北溫泉季11月1日至5日在北投地區盛大登場，今年溫泉季以名湯海灣宴潑湯祈"]}, {"name": "現以", "contents": ["北部人發現以前吃的都是南部粽時在想什麼", "我某朋友是個霸凌者", "分享一個我國中隔壁班轉學生的故事"]}, {"name": "參賽", "contents": ["若全民同意 > 走申請程序 > 中華奧會變更為臺灣奧會 > 參賽", "若全民同意 > 走申請程序 > 中華奧會變更為臺灣奧會 > 參賽", "上過國際談判桌的人都知道，這種重大的事件，中間要跑的流程很多"]}]
```
