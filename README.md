# websocket

WebSocket是雙向通訊模式，客戶端與伺服器之間只有在握手階段是使用HTTP協議的“請求-回應”模式互動，而一旦連線建立之後的通訊

則使用雙向模式互動，不論是客戶端還是服務端都可以隨時將資料傳送給對方

連線過程 —— 握手過程

1. 瀏覽器、伺服器建立TCP連線，進行三次握手。這是通訊的基礎，傳輸控制層，若失敗後續都無法執行。

2. TCP連線成功後，瀏覽器通過HTTP協議向伺服器傳送WebSocket支援的版本號等資訊。

3. 伺服器收到客戶端的握手請求後，同樣採用HTTP協議回饋資料。

4. 當收到了連線成功的訊息後，通過TCP通道進行傳輸通訊。

其中WebSocket在建立握手時，資料是通過HTTP傳輸的。但是建立之後，在真正傳輸時候是不需要HTTP協議的。

✒️websocket 系統網頁成品
---------------------------------------------
>程式部分:
>
>[test.html](https://github.com/shou0228/websocket/blob/99dd699201a34dc6b9750acecabc3ffb45052669/test.html)

>網頁呈現示意圖
![image](https://user-images.githubusercontent.com/68886395/158219035-41e2851e-657a-425f-b91a-c971823f4718.png)

✒️後端程式
---------------------------------------------
>python for websocket:
>
>[test.py](https://github.com/shou0228/websocket/blob/6c1fedcdfd7832a77efc17eba3f31932b5285106/test.py)
