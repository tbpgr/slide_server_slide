##  スライド開発・公開のワークフロー

1. yo reveal でスライド全体の土台を生成 <!-- .element: class="fragment roll-in" -->
1. bower install で関連ライブラリをインストール <!-- .element: class="fragment roll-in" -->
1. grunt serve でリアルタイムに編集・ブラウザ確認しながらスライドを作成 <!-- .element: class="fragment roll-in" -->
1. yo reveal:slide page_title --markdown でスライド追加 <!-- .element: class="fragment roll-in" -->
1. 追加したスライドのひな型を Markdown で手動編集 <!-- .element: class="fragment roll-in" -->
1. grunt dist でビルドを実行 <!-- .element: class="fragment roll-in" -->
1. dist ディレクトリに出力されたスライドの成果物を git で管理 <!-- .element: class="fragment roll-in" -->
1. スライドを GitLab に push <!-- .element: class="fragment roll-in" -->
1. GitLab の WebHook で Hubot に push を通知 <!-- .element: class="fragment roll-in" -->
1. Hubot が スライドサーバーのデプロイを実行 <!-- .element: class="fragment roll-in" -->
    1. git pull <!-- .element: class="fragment roll-in" -->
    1. forever start app.js <!-- .element: class="fragment roll-in" -->
1. Hubot が Kandan にスライドの push を通知 <!-- .element: class="fragment roll-in" -->

※まだまだ効率化の余地はあると思います <!-- .element: class="fragment roll-in" -->
