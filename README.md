# crypto-etf-flow
このレポジトリは https://farside.co.uk/ で公開されている暗号通貨ETFのフローに関するデータをcsv形式で保存しています。  

## データの取得方法
VPS上で稼働しているヘッドレスChromeとPythonでhtmlをパースしてcsv化しています。  
[GitHub - haturatu/curljs: DOM parsing using headless chrome](https://github.com/haturatu/curljs)  
を使用してhtmlを取得して標準出力に出力し、Pythonでパースしてcsv化しています。  

## データの更新
30mごとにcronで実行しています。  
差分があれば`git push`されます。  
