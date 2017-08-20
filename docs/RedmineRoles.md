ロールと権限
============

!!! note ""
    最終更新: 2016/04/03 [[原文](http://www.redmine.org/projects/redmine/wiki/RedmineRoles/19)]

ロールは、メンバーのプロジェクトにおける権限を定義します。プロジェクトの各々のメンバーは、そのプロジェクトにおけるロールが1個以上割り当てられます。プロジェクトが異なればユーザーに対して異なるロールを割り当てることができます。

ロールは新しく作成したり既存のものを編集したりできます。ロールは誰にも割り当てられていない場合に限り、削除できます。

ロールのプロパティ
------------------

-   **名前**: ロールの名称です。
-   **このロールにチケットを割り当て可能**: OFFにすると、このロールに所属するメンバーはチケットの担当者とすることができません (担当者の一覧に表示されません)
-   **表示できるチケット**: ロールに「チケットの表示」権限が割り当てられている場合、そのユーザーがどのチケットを参照できるのかは以下のルールが適用されます:
    -   *すべてのチケット* : すべてのチケットを参照できます
    -   *プライベートチケット以外*: プライベートチケット以外のチケットを参照できます。この選択肢がデフォルトです
    -   *作成者か担当者であるチケット*: そのユーザーが作成したか担当者であるチケットのみを参照できます

権限
----

ロールの編集画面で、チェックボックスをON/OFFすることにより権限の定義を行うことができます。

<table>
<thead>
<tr class="header">
<th>権限</th>
<th>説明</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><strong><em>プロジェクト</em></strong></td>
</tr>
<tr class="even">
<td>プロジェクトの追加</td>
<td>システム管理者ではないユーザーにプロジェクトの作成を許可<br />
プロジェクトを作成したユーザーが新しいプロジェクトでどのロールでメンバーになるのか、管理→設定→プロジェクトで設定できます</td>
</tr>
<tr class="odd">
<td>プロジェクトの編集</td>
<td>プロジェクトのプロパティの編集を許可</td>
</tr>
<tr class="even">
<td>モジュールの選択</td>
<td>プロジェクトのモジュールの有効/無効の切り替えを許可 (チケット、Wiki、リポジトリなど)</td>
</tr>
<tr class="odd">
<td>メンバーの管理</td>
<td>メンバーの追加/削除、メンバーのロールの変更を許可</td>
</tr>
<tr class="even">
<td>バージョンの管理</td>
<td>バージョンの追加/編集/削除を許可</td>
</tr>
<tr class="odd">
<td>サブプロジェクトの追加</td>
<td>そのプロジェクトにサブプロジェクトを追加することを許可</td>
</tr>
<tr class="even">
<td><strong><em>フォーラム</em></strong></td>
</tr>
<tr class="odd">
<td>フォーラムの管理</td>
<td>フォーラムの追加/編集/削除を許可</td>
</tr>
<tr class="even">
<td>メッセージの追加</td>
<td>フォーラムで新しいトピックの投稿を許可</td>
</tr>
<tr class="odd">
<td>メッセージの編集</td>
<td>任意のメッセージの編集と任意メッセージの添付ファイル削除を許可</td>
</tr>
<tr class="even">
<td>自身が記入したメッセージの編集</td>
<td>自分が投稿したメッセージの編集を許可</td>
</tr>
<tr class="odd">
<td>メッセージの削除</td>
<td>任意のトピックと返信の削除を許可</td>
</tr>
<tr class="even">
<td>自身が記入したメッセージの削除</td>
<td>自分が投稿したトピックと返信の削除を許可</td>
</tr>
<tr class="odd">
<td><strong><em>文書</em></strong></td>
</tr>
<tr class="even">
<td>文書の追加</td>
<td>プロジェクトの文書の追加を許可</td>
</tr>
<tr class="odd">
<td>文書の編集</td>
<td>プロジェクトの文書の編集を許可</td>
</tr>
<tr class="even">
<td>文書の削除</td>
<td>プロジェクトの文書の削除を許可</td>
</tr>
<tr class="odd">
<td>文書の閲覧</td>
<td>プロジェクトの文書の表示を許可</td>
</tr>
<tr class="even">
<td><strong><em>ファイル</em></strong></td>
</tr>
<tr class="odd">
<td>ファイルの管理</td>
<td>プロジェクトの「ファイル」モジュールにおいてファイルの追加/編集/削除を許可</td>
</tr>
<tr class="even">
<td>ファイルの閲覧</td>
<td>ファイルの参照を許可</td>
</tr>
<tr class="odd">
<td><strong><em>チケットトラッキング</em></strong></td>
</tr>
<tr class="even">
<td>チケットのカテゴリの管理</td>
<td>チケットのカテゴリの追加/編集/削除を許可</td>
</tr>
<tr class="odd">
<td>チケットの閲覧</td>
<td>チケットの参照を許可</td>
</tr>
<tr class="even">
<td>チケットの追加</td>
<td>新しいチケットの作成を許可</td>
</tr>
<tr class="odd">
<td>チケットの編集</td>
<td>既存のチケットのあらゆる項目の編集を許可</td>
</tr>
<tr class="even">
<td>チケットのコピー</td>
<td>既存のチケットのコピーを許可</td>
</tr>
<tr class="odd">
<td>関連するチケットの管理</td>
<td>チケット同士の関連の追加/削除を許可</td>
</tr>
<tr class="even">
<td>子チケットの管理</td>
<td>チケットへの子チケット追加/削除を許可</td>
</tr>
<tr class="odd">
<td>注記の追加</td>
<td>既存のチケットに対して注記の追加を許可</td>
</tr>
<tr class="even">
<td>注記の編集</td>
<td>既存チケットのすべての注記の編集を許可</td>
</tr>
<tr class="odd">
<td>自身が記入した注記の編集</td>
<td>自分の注記のみ編集を許可</td>
</tr>
<tr class="even">
<td>チケットの削除</td>
<td>チケットの削除を許可</td>
</tr>
<tr class="odd">
<td>公開クエリの管理</td>
<td>全ユーザー向けのクエリの追加/編集/削除を許可</td>
</tr>
<tr class="even">
<td>クエリの保存</td>
<td>自分専用のクエリの保存を許可</td>
</tr>
<tr class="odd">
<td>ガントチャートの閲覧</td>
<td>ガントチャートの表示を許可</td>
</tr>
<tr class="even">
<td>カレンダーの閲覧</td>
<td>カレンダーの表示を許可</td>
</tr>
<tr class="odd">
<td>ウォッチャー一覧の閲覧</td>
<td>チケットのウォッチャーの一覧を参照することを許可</td>
</tr>
<tr class="even">
<td>ウォッチャーの追加</td>
<td>他のユーザーをチケットのウォッチャーに追加することを許可</td>
</tr>
<tr class="odd">
<td>ウォッチャーの削除</td>
<td>ウォッチャーの削除を許可</td>
</tr>
<tr class="even">
<td><strong><em>ニュース</em></strong></td>
</tr>
<tr class="odd">
<td>ニュースの管理</td>
<td>プロジェクトのニュースの追加/編集/削除を許可</td>
</tr>
<tr class="even">
<td>ニュースへのコメント</td>
<td>ニュースにコメントを追加することを許可</td>
</tr>
<tr class="odd">
<td><strong><em>リポジトリ</em></strong></td>
</tr>
<tr class="even">
<td>リポジトリの管理</td>
<td>プロジェクトのリポジトリの設定を許可</td>
</tr>
<tr class="odd">
<td>リポジトリの閲覧</td>
<td>プロジェクトのリポジトリの参照を許可</td>
</tr>
<tr class="even">
<td>更新履歴の閲覧</td>
<td>チェンジセットの参照を許可</td>
</tr>
<tr class="odd">
<td>コミット権限</td>
<td>Redmine.pm でプロジェクトのリポジトリへの書き込みを許可<br />
<a href="http://www.redmine.org/projects/redmine/wiki/Repositories_access_control_with_apache_mod_dav_svn_and_mod_perl">Repositories access control with apache, mod_dav_svn and mod_perl</a> 参照</td>
</tr>
<tr class="even">
<td><strong><em>時間管理</em></strong></td>
</tr>
<tr class="odd">
<td>作業時間の記入</td>
<td>作業時間の記録を許可</td>
</tr>
<tr class="even">
<td>作業時間の閲覧</td>
<td>作業時間の参照を許可</td>
</tr>
<tr class="odd">
<td>作業時間の編集</td>
<td>任意の作業時間の編集を許可</td>
</tr>
<tr class="even">
<td>自身が記入した作業時間の編集</td>
<td>自分が記録した作業時間のみ編集を許可</td>
</tr>
<tr class="odd">
<td>作業分類 (時間管理) の管理</td>
<td>作業分類 (時間管理)の追加/編集/削除を許可</td>
</tr>
<tr class="even">
<td><strong><em>Wiki</em></strong></td>
</tr>
<tr class="odd">
<td>Wikiの管理</td>
<td>Wikiの追加/削除を許可<br />
Wikiの削除は <strong>取り消しできない操作</strong> です。すべてのページ、履歴、添付ファイルが削除されます!</td>
</tr>
<tr class="even">
<td>Wikiページ名の変更</td>
<td>既存のWikiページの名前の変更および親ページの割り当てを許可</td>
</tr>
<tr class="odd">
<td>Wikiページの削除</td>
<td>Wikiページの削除を許可<br />
Wikiページの削除は <strong>取り消しできない操作</strong> です。そのページと履歴が削除されます!</td>
</tr>
<tr class="even">
<td>Wikiの閲覧</td>
<td>Wikiの参照を許可</td>
</tr>
<tr class="odd">
<td>Wikiページを他の形式にエクスポート</td>
<td>Wikiページの他の形式でのエクスポートを許可 (pdf, htmlなど)</td>
</tr>
<tr class="even">
<td>Wiki履歴の閲覧</td>
<td>Wikiページの古いバージョンやバージョン間の差分の参照を許可</td>
</tr>
<tr class="odd">
<td>Wikiページの編集</td>
<td>凍結されていないWikiページの編集を許可</td>
</tr>
<tr class="even">
<td>添付ファイルの削除</td>
<td>Wikiページに添付されたファイルの削除を許可</td>
</tr>
<tr class="odd">
<td>Wikiページの凍結</td>
<td>Wikiページのロック・アンロックとロックされたページの編集を許可</td>
</tr>
</tbody>
</table>

システムロール
--------------

Redmineには二つのシステムロール: 「非メンバー」と「匿名ユーザー」があります。これらはRedmine内部で使用されるものであり、削除することはできません。

-   **非メンバー**: 登録されているユーザーが、メンバーとなっていないプロジェクトにアクセスするときに適用される権限を定義します。
-   **匿名ユーザー**: 匿名ユーザー(ログインしていないユーザー)の権限を定義します。

これらのロールは公開プロジェクトに対してのみ適用されます。匿名ユーザーとメンバーではないユーザーは公開プロジェクトでなければアクセスできないためです。

一部の権限はこれらのロールに割り当てることができません（例: 「メンバーの管理」権限)。