# 概要

* ModalDialogからwindow.openへ移行作業を行う際のサンプル。

# 実装内容

* 呼び出し元のウィンドウに高さ100%/幅100%のDIVを設定し、style disyplayを操作し、操作不能、操作可能及びグレーアウトを実現している。フレームの場合はすべてのフレームに設定すれば可能。

# 注意事項

* フォーカスの固定については実現不能。
    * 1秒毎に小窓へフォーカスを戻す処理を実装し、コメントアウトしているがかなりの力技感がでている。

# 参考資料

* [JavaScript window.open: Display Modal Popup Window](https://www.aspsnippets.com/Articles/JavaScript-windowopen-Display-Modal-Popup-Window.aspx)
* [window.openでモーダルぽくする](https://qiita.com/bassyaroo/items/6566d06e27fdd970dc01)

# 確認環境

* OS:Window 10 Pro 21H2
* Browser
    * Chrome 102.0.5005.63
    * Microsoft Edge 102.0.1245.33
* Visual Studio Code
    * Live Server

# 今回触れなかった代替実装について

* Html 5.2以降提供されているdialogエレメントを使用した実装方法。
    * ウィンドウの外に出せないためフレームタイプの画面には向かない。
    * 非同期処理でdialog#showModalが動いてしまうためcallback実装が不可欠。
* jQuery ui dialogを使用した実装方法。
    * ウィンドウの外に出せないためフレームタイプの画面には向かない。
    * 非同期処理で動いてしまうためcallback実装またはPromise実装が必要。
