# Moodleブロックテンプレート

このテンプレートは、Moodleのブロック用のテンプレートです。

* このテンプレートは、デフォルトでテキストコンテンツタイプを使用するブロックを想定しています。リストアイテムを表示するブロック（$this->content->items と $this->content->icons を使用）を作成したい場合は、ブロックの継承クラスを `block_base` から `block_list` に変更してください。詳細については、https://docs.moodle.org/dev/Blocks#Additional_Content_Types を参照してください。

* 設定 > サイト管理 > 開発 > XMLDBエディタ に移動し、モジュールのテーブルを修正してください。

* version.phpを修正し、モジュールの初期バージョンを設定してください。

* 設定 > サイト管理 > 通知 に移動すると、モジュールのテーブルが正常に作成されたことが確認できるはずです。

* サイト管理 > プラグイン > ブロック > ブロック管理 に移動すると、このnewblockがインストール済みモジュールのリストに追加されていることが確認できるはずです。

* これで、モジュールの開発を始めることができます。最初のステップとして、block_newmodule.phpとedit_form.phpを修正することをお勧めします。機能を追加するには、db/access.phpを確認してください。

コードと経験を共有することをお勧めします - http://moodle.org にアクセスしてください。

頑張ってください！


---

このテンプレートは [danielneis/moodle-block_newblock](https://github.com/danielneis/moodle-block_newblock) を基に作成されています。
