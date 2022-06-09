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
