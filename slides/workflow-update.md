##  スライド修正・更新のワークフロー

1. 開発環境でスライドを編集 <!-- .element: class="fragment roll-in" -->
1. grunt dist でビルドを実行 <!-- .element: class="fragment roll-in" -->
1. dist ディレクトリに出力されたスライドの成果物を git commit <!-- .element: class="fragment roll-in" -->
1. スライドを GitLab に push <!-- .element: class="fragment roll-in" -->
1. GitLab の WebHook で Hubot に push を通知 <!-- .element: class="fragment roll-in" -->
1. Hubot が スライドサーバーのデプロイを実行 <!-- .element: class="fragment roll-in" -->
    1. git pull <!-- .element: class="fragment roll-in" -->
1. Hubot が Kandan にスライドの push を通知 <!-- .element: class="fragment roll-in" -->
