* STEP1
  baseconnect.inからスクレイピングして

* STEP2
  mapboxで住所を緯度経度に変換

* STEP3
  mapboxでプロット

* STEP4
  CTO協会加盟企業リストをスクレイピング取得する
  - ログイン不要で、サーバサイドでHTTPClientにて実装できるか?
    - 実装できる
      - firebase function上でnodejsにて、puppeteerでやりたい
        - firebase functionだと無料ではできない
      - gigalixir, elixir, crawly, postgresにする
        - CTO協会加盟企業リストをAPI経由で配信できるようにする
* STEP5
  CTO協会加盟企業ごとのTechブログマスターを作成
  ・企業名
  ・企業のテックブログURL

* コロナ
   - http://who.maps.arcgis.com/home/item.html?id=0027e4bc143d4daeb1236eb2e613dc94&view=list#data
   
* STEP6
  CTO協会加盟企業ごとのキー Twitterアカウントマスターを作成
  ・企業名
  ・タグ default, cto
  ・Twitterアカウント名

* STEP7
  TwitterOAuth認証をクリアする

* STEP8
  東京都のリアルタイム交通データをGTFS realtimeプロトコル形式で取得する

* STEP9
  mapboxをreact化する

* STEP10 STEP6, 

* STEP7
  mapboxを3D化する

