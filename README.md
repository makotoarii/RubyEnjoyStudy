## プログラミングガイドライン

- 目的
- 命名規則（禁止事項含む）

# 目的
- 【 コードを共通化する。それにより、可読性を上げる。】

# 命名規則
- 【 変数名は小文字で_区切る原則snake_case 】
- - OK:
- names
- cart_item
- order_id
- order_idをoidのように省略しすぎるのは非推奨。とはいえ例えばPostgreSQLのOIDはoidとしても構わない。

- - NG:
- cartItem
- order_Id

- ※例外的に短い名前が使われるものもあるが、あくまで例外で、どちらかと言うと長めの命名の方が多い。

- 【 定数は全部大文字で_区切り 】
- - OK:
- FIGURE_X_SIZE
- MAX_WIDTH

- - NG:
- Figure_X_Size
- MaxWidth

- 【 真偽値を返すメソッドには?をつける。isやhasを頭につけたりしない 】
- - OK:
- - user?
- - permitted?
- - clicked?

- - NG:
- - is_user
- - is_user?
- - user_p
- - is_clicked

- 【 メソッド名は小文字で_区切る原則snake_case 】
- - OK:
- - find_items
- - all_children

- - NG:
- - findItems
- - find_Items
- - FindItems
- - Find

- 【 クラス名、モジュール名は原則CamelCase 】
- - OK:
- - Groups
- - ColorBar
- - CoinServer

- - NG：
- - GROUPS
- - COLORBar
- - Coin_Server

- 【 その他の変数 】
- - i, j（ループカウンタやインデックス用）
- - x, y, z（座標用）

# 文字列
- 【 文字列は文字列中に特殊文字を含めることを前提として、基本「""」ダブルクォーテーションで囲む

# メソッド
- 【「printメソッド」は実行結果やメッセージなどをそのまま表示したいときに使用する 】
- 【「pメソッド」は実行中のプログラムの様子を確認したい（オブジェクトの型をそのまま表示）ときに使用する 】
- 【「putsメソッド」は改行したいときにシンプルに書くことができて「\n」の特殊文字が必要ないため、基本putsメソッドを使う 】

# タブ
- 基本的にタブのスペースは「半角2文字」分とする
