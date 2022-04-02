
　プラグイン『BalloonSelector』

　作成者　　　　Don
　一次配布元　　http://nikolat.herokuapp.com/

■機能

　インストール済みのバルーン画像を一部切り取ってバルーン内に９個表示します。
　バルーンを選択するとそのバルーンに切り替わります。

■仕様

◆Ghost側に通知されるイベントは以下の通りです。

●OnBalloonSelectMenu
Reference0　　バルーンを表示するページ番号(Zero Origin)

　バルーンセレクトメニューを表示する際に通知されます。
　バルーン内に表示されているページ番号より１小さい値です。

●OnBalloonSelectExec
Reference0　　バルーン名

　ユーザがバルーンを選択した際、バルーンチェンジする時に通知されます。

●OnBalloonSelectCancel

　ユーザがバルーンセレクトメニューを閉じた際に通知されます。
　バルーンブレイク時も同様の扱いとします。

◆Ghost側から利用できるイベントは以下の通りです。
（\![raiseplugin,BalloonSelector,イベント名,Argument0,...]）

●OnMenuExec

　バルーンセレクトメニューの最初のページを開きます。

●OnBalloonSelectMenuOpen
Argument0　　バルーンを表示するページ番号(Zero Origin)

　バルーンセレクトメニューをページ番号を指定して表示します。
　バルーン内に表示されるページ番号より１小さい値を指定してください。

■謝辞

　◆YAYA as PLUGINを使わせて頂いております。
　◇「整備班 -The Maintenance Shop-」
　　http://ms.shillest.net/yaya_as.xhtml

　ありがとうございます。

■更新履歴

2008/09/07	Ver1.0	新規作成
2008/09/08	Ver1.1	バルーンサイズに合わせて変形できるようにした
          	      	OnBalloonSelectMenuOpen追加
2008/09/09	Ver1.2	バルーンフォルダを複数指定した場合に対応
2008/09/10	Ver1.3	バルーンの自動スクロールを無効化
          	      	バルーンタイムアウト無効化
          	      	バルーンブレイクをOnBalloonSelectCancelとして通知
          	      	現在のページを下段ページボタンに反映
          	      	下段ページボタンの最大表示数を30とした
          	      	バルーン切り取りサイズの最小値を設定
          	      	全体的なレイアウトの微調整
2008/09/13	Ver1.4	文字コードがShift_JIS以外に対応できていなかったのを修正
2008/09/14	Ver1.5	yaya.dll差し替え
          	      	YAYA as PLUGINテンプレート差し替え
2008/12/14	Ver1.6	yaya.dll差し替え
          	      	YAYAの多言語化によりShift_JIS / UTF-8以外にも多くの文字コードに対応可能に
2011/02/07	Ver1.7	トランスレートを行うゴーストで意図しない文字列の置換が行われる
          	      	場合がある不具合の修正
2021/10/23	Ver1.8	yaya.dll差し替え
          	      	ネットワーク更新先の変更
2021/12/15	Ver1.9	yaya.dll差し替え
          	      	システム辞書微修正
2022/04/02	Ver2.0	yaya.dll差し替え
          	      	システム辞書微修正
