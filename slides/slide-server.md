## スライドサーバー

* 内部利用目的なので手間をかけない構成で! <!-- .element: class="fragment roll-in" -->
* node.js + npm + connect + forever <!-- .element: class="fragment roll-in" -->
* connect => ミドルウェアフレームワーク。  
簡易httpサーバーとして利用 <!-- .element: class="fragment roll-in" -->
* forever => connect のデーモン化に利用 <!-- .element: class="fragment roll-in" -->
* install <!-- .element: class="fragment roll-in" -->
    ~~~bash
    sudo apt-get install -y nodejs
    sudo apt-get install -y npm
    sudo npm install forever -g
    sudo npm install connect
    ~~~
    <!-- .element: class="fragment roll-in" -->

* サーバーのコードはこれだけ <!-- .element: class="fragment roll-in" -->
    ~~~javascript
    var connect = require('connect');
    connect.createServer(
        connect.static(__dirname)
    ).listen(3000); // お好みのポートで。
    ~~~
    <!-- .element: class="fragment roll-in" -->
