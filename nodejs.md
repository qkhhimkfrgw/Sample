# supervisorでサーバを起動するなら、ソースが変えられた時に自動再起動できる #

### インストール ###

	npm -g install supervisor

### 実行 ###

	d:
	cd NodeTest
	supervisor debug index.js
  
または
  
	d:  
	cd D:\ExpressNodeProject  
	npm start

デバッグの場合は
  
	d:
	cd NodeTest
	node debug index.js


# nodeでデバッグ #

### ステップ ###

1.  先ず、デバッグしたいところで`debugger`を付けておく    
* CMDで`node server`を起動  
* もう一つのCMDで`node-inspector`を実行

ソース

    d:
    cd NodeTest  
    node --debug index.js

または

	d:  
	cd NodeTest  
	node-inspector --web-port=8888


### 訪問方法 ###

	127.0.0.1:8888/debug?port=5858

# expressのインストール(expressはlightweight-frameworkである) #

	npm install -g express
	npm install -g express@3  // 第三版という意味
	npm install -g express-generator  // expressプロジェクト作成ツール

### expressバージョーン：  
	express -V

### expressプロジェクト作成ステップ：
1. フォルダーで`express projeceName`を入力して実行する
*  `cd projeceName`をプロジェクトフォルダに入る
*  `npm install`を入力して依存ファイルを追加する
*  `npm start`を入力し、サーバを起動させる(旧いバージョーンでは`node app.js`で起動)
*  `localhost:3000`を訪問する

# デバッグ手順

1. `node --debug-brk xxx.js`をデバッグ環境として実行し、appの最初のところにブレークする
*  `node-inspector &`をデバッグ挿入する
*  `http://127.0.0.1:8080/debug?port=5858`でchromeのデバッグ窓口のような画面を開くと、デバッグできる
*  `http://localhost:8888/`でウェブを訪問する

# Jadeテンプレート #
