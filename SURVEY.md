
* 自分で都合できる時間を確保
* 自分の興味関心に基づいて行動し、人の役に立ちそうなことに関連付ける。
* ２０１８年よりも１段階戦略的に情報蒐集したり行動したり出来るようになりたい
* 目立つ看板を立てる。


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


# 行動意思決定基準

## 現在
* 社会貢献
  - 自分 < 優先度 < 自分以外
* 用途・目的重視
  - 技術的関心 < 優先度 < プロジェクト・用途
* 運用重視
  - プロダクト開発(front/serverside) <  優先度 < インフラ基盤強化・運用設計

## 変更後(全て逆転させる)

* 自己満足
  - 自分 > 優先度 > 自分以外
* 技術重視
  - 技術的関心 < 優先度 < プロジェクト・用途
* 運用重視
  - プロダクト開発(front/serverside) <  優先度 < インフラ基盤強化・運用設計
