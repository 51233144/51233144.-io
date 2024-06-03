Title: WCM 五專第五週課程內容
Date: 2024-03-18 11:00
Category: 五專
Tags: Chatgpt, w5
Slug: wcm-5j-w5
Author: kmol
---
Title: WCM 五專第四週課程內容 Date: 2024-03-11 11:00 Category: 五專 Tags: 計概, 分組, w4 Slug: wcm-5j-w4 Author: kmol
以下為五專精密機械科網際內容管理課程第四週上課內容, 包括回顧計算機概論, 以及如何在網頁推送至 Github 倉儲之前檢查所編輯的網頁內容.

建立個人最短網址網站
Github Pages服務可以讓 Github 帳號的擁有者, 使用"帳號.github.io"作為倉儲名稱, Github 會自動將此網站設定 Github Pages, 假如此倉儲內部帶有超文件, 則此倉儲對應的網址將會是 https://帳號.github.io

說明如何建立短網址的 Github Pages 網站教學影片

下載 main2.txt 與 static.txt, 其中包含 main2.py 與 static.py, 只要在 Shell 執行 python3 main2.py 就可以執行倉儲內的靜態網站檢視. 另一方面, 若要取消先前執行 python3 main2.py, 只需要在 Shell 頁面按下 ctrl + c, c 代表 cancle 也就是取消. 然後若要執行動態網站，可以在 Shell 執行 python3 main.py 或者使用 Replit 的 Run 按鍵.

說明如何在 Replit 檢視靜態網站教學影片

說明如何下載 replit_main2.7z 並在倉儲中建立兩個檔案教學影片

以上為第四週進度

Foosball 與影像辨識
有關 Foosball

History of Foosball

Raspberry Pi

40623128

40623130

airhockey

https://github.com/mdecycu/foosball_robot

OBS 錄影與直播
https://obsproject.com/ 是一套自由開放原始碼的錄影與直播套件. 在 Windows 操作系統可以使用可攜模式 執行.

開啟 Y:\obs\bin\64bit\obs64.exe 後, 可以選擇串流或錄影優先模式, 並在"設定"中的"一般"下的"語言"選擇使用 English 後, 重新啟動就可顯示英文語系畫面.

Windows 操作系統中的 OBS 設定內容存放於 C:\Users\使用者帳號\AppData\Roaming\obs-studio 目錄中, 若將 OBS 放在 USB 隨身碟中, 希望每次開啟可攜程式系統都能保有先前的設定, 可以利用下列批次指令, 將 USB 隨身碟中所儲存的先前設定複製到 Windows 目錄.

    REM Xcopy %Disk%:\home_ipv6\AppData\Roaming\obs-studio C:\users\%USERNAME%\AppData\Roaming\obs-studio /E /H /C /I /Y
在 Windows 命令列視窗中, 可以使用 xcopy /? 查詢與 xcopy 指令有關的選項設定說明.

OBS 支援多 Scenes(場景), 且每一個場景支援多個 Sources(來源), 若要錄製電腦操作畫面, 可以選擇 Display Capture 作為 Source, 之後設定 Audio, Video, Output 以及 Hotkeys, 就可以開始錄影.

ShareX 錄影與截圖
在 Windows 操作系統中, 若無直播需求, 且僅需錄製電腦的操作流程或截圖, 可以使用 ShareX

wcm2024 網站如何整合 https://github.com/nextapps-de/spotlight and https://github.com/xemle/home-gallery?

Python 與 ffmpeg.exe 結合成為影像讀取工具: https://github.com/chenxinfeng4/ffmpegcv

除了 Replit, 還可以使用 Codespaces, Gitpod 與隨身系統維護 wcm2024 網站內容.

Replit 免費帳號並沒有線上工作時間限制(但給定的運算資源較小), Codespaces 免費帳號每個月可以使用 120 core hours(優點是直接與 Github 帳號綁定), Gitpod 免費帳號每個月可以使用 50 hours(優點是開放原始碼, 且給定運算資源最多), 使用隨身程式系統則可在沒有網路連線時進行改版, 有網路連線時才將近端的版本推到 Github 倉儲.

#計算機概論摘要 ASUS Product Guide

Computing Trend Report

AI Trend Report

高中計概

大學計概

Github Pages 參考網站 (倉儲) (相關影片)

如何利用 OBS download + 網際簡報進行直播同時錄影?

nslookup 與 tracert
nslookup - name server lookup 符號名稱伺服器查詢

tracert - trace route 路由追蹤

利用 codespaces 維護 wcm2024 網站內容
一般所謂網站, 指的是 www (world wide web) 全球資訊網協定中的 html 超文件檔案資料, 可以直接用網頁瀏覽器在近端開啟, 或放在 www 伺服器上, 由網頁瀏覽器透過網址連線後觀看網頁內容.

網頁的組成 - 請用瀏覽器連結到一個網站, 然後用滑鼠右鍵帶出 Chrome 瀏覽器的"檢視頁面來源", 查看該網頁有哪些超文件標註內容.

建立網頁內容
由於採直接編寫 html 建立網頁的方法比較繁瑣, 因此在網際內容管理課程中, 運用 Python 程式編寫了一套系統, 用來協助使用者建立網站內容.

當使用者在建立網站過程, 資料不斷被納入, 雖然可以利用章節對內容分類, 但在網站內容完成之前, 使用者無法依照內容建構的時間先後次序, 主題式閱讀網站資料, 因此除了章節式的網站內容之外, 可以採流水帳的方式建立網站內容, 一般稱依照時間先後次序編寫網站文章的方式為"網誌" (Weblog).

如何在 Replit 中建立並維護個人或分組的網站內容?

建立網誌內容
網際內容管理課程建立 Pelican 建構, 並且利用 Markdown 格式編寫之後, 再利用轉檔流程轉為 html.

如何在 Replit 中設定並建立個人網站中的網誌內容?

針對以上課程內容, 請利用以下留言系統進行討論:

Please enable JavaScript to view the comments powered by Disqus.