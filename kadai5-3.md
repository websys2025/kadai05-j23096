## 外部APIの呼び出しのミニレポート
### Q3-1. 郵便番号APIについて説明せよ。
* エンドポイントと機能
　endpoint = "https://zipcloud.ibsnet.co.jp/api/search";
　　
* リクエストとレスポンスのフォーマット
　
　https://zipcloud.ibsnet.co.jp/api/search?zipcode=郵便番号

　Response {type: 'cors', url: 'https://zipcloud.ibsnet.co.jp/api/search?zipcode=1310045', redirected: 　false, status: 200, ok: true, …}
　
　message: null, results: Array(1), status: 200}
　kadai5-1.html:23
　message =null
　results =(1) [{…}]
　0 ={address1: '東京都', address2: '墨田区', address3: '押上', kana1: 'ﾄｳｷｮｳﾄ', kana2: 'ｽﾐﾀﾞｸ', …}
### Q3-2. 各自で調査したAPIについて説明せよ。
* APIの名称と参照URL
　猫情報API
　参照URL　：　https://catfact.ninja/fact
* エンドポイントと機能
　https://catfact.ninja/fact　猫のの雑学を取得する

* リクエストとレスポンスのフォーマット
 "https://catfact.ninja/fact?max_length=最大文字列数"

 ｛fact: 猫の雑学｝
### Q3-3. 感想
* 今回の課題で苦労したこと
　zipcloudを動かすためにFormから入力した内容をURLに結びつけること
　公式サイトを見に行ってやっと理解できた。
* 演習を通して理解できたこと
　外部APIをfetchで呼び出すこと。
　それぞれのAPIから受け取った結果のフォーマットを確認してプログラムに適応させる必要があること
* Web APIの利便性や課題など
　利便性：　特定の場所を入力するだけで色々な結果を表示できる。
　課題：フォーマットを確認しないと使えない
