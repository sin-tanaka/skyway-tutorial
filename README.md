# skyway-tutorial

https://webrtc.ecl.ntt.com/js-tutorial.html の写経

[DEMO](https://sin-tanaka.github.io/skyway-tutorial/)

## 覚え書き

iOS Safariだと一部追加対応が必要

https://support.skyway.io/hc/ja/articles/115012750968-Safari%E3%81%B8%E3%81%AE%E5%AF%BE%E5%BF%9C%E7%8A%B6%E6%B3%81

* video要素に `position: -webkit-sticky;` を追加する
* video属性に `playsinline` を指定する
* `.play()` で再生する


## 参考

[SkyWay JavaScript SDK API リファレンス](https://webrtc.ecl.ntt.com/js-reference/)

[相手Peerの切断検知について](https://support.skyway.io/hc/ja/community/posts/115009364108-%E7%9B%B8%E6%89%8BPeer%E3%81%AE%E5%88%87%E6%96%AD%E6%A4%9C%E7%9F%A5%E3%81%AB%E3%81%A4%E3%81%84%E3%81%A6)

Connectionのcloseイベントが呼ばれるのはPeer disconnectedが走って一定時間後っぽい?  
→ DataConnectionも立てて、send('hoge')でDataConnection.dataイベントを発火させてあげればリニアに接続切れるけど。。。
