カスタムフィールド
==================

!!! note ""
    最終更新: 2015/08/19

カスタムフィールドを使うとRedmineの様々な型のデータに追加の情報を加えることができます。

カスタムフィールドの型
----------------------

-   **整数**: 正または負の値
-   **テキスト**: 一行の文字列
-   **長いテキスト**: 複数行にわたる文字列
-   **日付**: 日付
-   **真偽値**: チェックボックス
-   **リストから選択**: ドロップダウンリスト
-   **ユーザ**: プロジェクトに参加しているメンバー
-   **バージョン**: プロジェクトに登録されているバージョン

各々のカスタムフィールドで妥当性検査を行うことができます:

-   **最小値 - 最大値の長さ** : フィールドの長さの最小値・最大値(0の場合は制限無し)
-   **正規表現** : フィールドの内容を検査するのに使用する正規表現

例:

`^\[A-Z]{4}\d+$` : アルファベット大文字4文字と、後続する４桁の数字

`^[^0-9]*$` : 文字列（数字を含まない）

利用可能な正規表現は、[Rubyのリファレンス](http://doc.ruby-lang.org/ja/1.8.7/doc/spec=2fregexp.html) で確認できます。

-   **選択肢**: "リストから選択"フィールドで利用可能な選択肢です。値を一行ずつ記述します。

カスタムフィードに対する設定
----------------------------

### チケット

チケットのカスタムフィールドは、チケット、チケット一覧、カスタムクエリ、作業時間の記録画面で利用・参照できます。

-   **トラッカー**:
-   **必須**: ONにすると、チケットの登録・更新時の必須項目になります。
-   **全プロジェクト向け**: ONにすると、このカスタムフィールドはすべてのプロジェクトのチケットで使われます。OFFにすると、個々のプロジェクトでこのカスタムフィールドを使用するかどうか選択できます。 ([プロジェクトの設定](RedmineProjectSettings) を参照).
-   **フィルタとして使用**:
-   **検索対象**: Redmineの検索機能で検索可能になります ([検索](RedmineSearch) を参照)

### 作業時間の記録

「作業時間の記録」のカスタムフィールドは、作業時間の記録画面で利用／参照できます。

-   **必須**: ONにすると、作業時間の登録・更新時の必須項目になります。

### プロジェクト

プロジェクトのカスタムフィールドは、各プロジェクトの「概要」画面で利用・参照できます。

-   **必須**: ONにすると、プロジェクトの作成・保存時の必須項目になります。
-   **検索条件に設定可能とする**: Redmineの検索機能で検索可能になります ([検索](RedmineSearch) を参照)

### バージョン

バージョンのカスタムフィールドはロードマップ画面および個別のバージョンの表示画面で利用・参照できます。

-   **必須**: ONにすると、バージョンの登録・更新時の必須項目になります。

### ユーザー

ユーザーのカスタムフィールドはユーザー情報画面で利用・参照できます。

-   **必須**: ONにすると、ユーザーの作成・保存時の必須項目になります。
-   **編集可能**: 自分のアカウントの情報を各ユーザーが編集可能になります。

### グループ

**注意**: グループのカスタムフィールドは現時点ではRedmine本体では使われていませんが、プラグインやテーマの中には利用しているものがあるかもしれません。ここでの設定は現在のバージョンのRedmineの動作には何の影響も及ぼしません。

### 作業分類 (時間トラッキング)

作業分類のカスタムフィールドは作業時間の記録画面とプロジェクトの設定画面で利用・参照できます。この機能の詳細については [#4077](http://www.redmine.org/issues/4077) もあわせて参照してください。

-   **必須**: ONにすると、作業分類の登録・更新時の必須項目になります。

### チケットの優先度

**注意**: チケットの優先度のカスタムフィールドは現時点ではRedmine本体では使われていませんが、プラグインやテーマの中には利用しているものがあるかもしれません。ここでの設定は現在のバージョンのRedmineの動作には何の影響も及ぼしません。

### 文書カテゴリ

**注意**: 文書カテゴリのカスタムフィールドは現時点ではRedmine本体では使われていませんが、プラグインやテーマの中には利用しているものがあるかもしれません。ここでの設定は現在のバージョンのRedmineの動作には何の影響も及ぼしません。