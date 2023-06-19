# Laravel 10 帶有文件的規劃行程具象狀態傳輸應用程式介面

根據客戶的假期時間（如果是多人一起旅行需要綜合大家共同的休息時間），參考旅行目的地的天氣情況以及最佳旅遊時間，規劃旅行時間，包括：出發時間、返回時間以及行程。

## 使用方式
- 把整個專案複製一份到你的電腦裡，這裡指的「內容」不是只有檔案，而是指所有整個專案的歷史紀錄、分支、標籤等內容都會複製一份下來。
```sh
$ git clone
```
- 將 __.env.example__ 檔案重新命名成 __.env__，如果應用程式金鑰沒有被設定的話，你的使用者 sessions 和其他加密的資料都是不安全的！
- 當你的專案中已經有 composer.lock，可以直接執行指令以讓 Composer 安裝 composer.lock 中指定的套件及版本。
```sh
$ composer install
```
- 產生 Laravel 要使用的一組 32 字元長度的隨機字串 APP_KEY 並存在 .env 內。
```sh
$ php artisan key:generate
```
- 執行 __Artisan__ 指令的 __migrate__ 來執行所有未完成的遷移。
```sh
$ php artisan migrate
```
- 運行功能測試。功能測試可以測試大部分的程式碼，包含一些物件如何進行互動，甚至是完整的 HTTP 請求到一個 JSON 端點。
```sh
$ php artisan test
```
- 執行 __Artisan__ 指令的 __scribe:generate__ 來執行 API 文件產生。
```sh
$ php artisan scribe:generate
```
- 在瀏覽器中輸入已定義的路由 URL 來訪問，例如：http://127.0.0.1:8000。
- 你可以經由 `/docs` 來進行應用程式介面文件閱讀。

----

## 畫面截圖
![](https://i.imgur.com/7xMKSwZ.png)
> 檢查程式碼是否如預期般執行

![](https://i.imgur.com/kq51Yga.png)
> 建議找不同領域或程度的開發者來閱讀文件，確認文件的內容適合任何程度的人閱讀