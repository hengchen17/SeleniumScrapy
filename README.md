# SeleniumScrapy

用 `requests` + `BeautifulSoup` 爬取亞洲大學資工系教師頁面,整理每位老師的專長,輸出 JSON / TXT / CSV。

> 目前尚未使用 Selenium,靜態頁面用 requests 即可;若日後遇到需要 JS 渲染的頁面再引入。

## 使用

```bash
pip install -r requirements.txt
python scrape_faculty_expertise.py
```

輸出檔案:`asia_csie_faculty_expertise.json` / `.txt` / `.csv`。

## 注意

- 網頁結構(`.et_pb_team_member`)改版後選擇器需同步調整。
- 爬取前請確認網站使用條款,並控制請求頻率。
