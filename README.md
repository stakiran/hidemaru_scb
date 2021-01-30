# hidemaru_scb
秀丸エディタでScrapbox風味の記法やリンクを実現する

## 要件
- 秀丸エディタ V8.00 以上

## インストール
強調表示とマクロの設定が必要です。

### 強調表示の設定
- 1: その他 > ファイルタイプ別の設定 > 設定のリストより、拡張子 `.scb` 用の設定を一つ新たにつくる
- 2: .scb ファイルに対して 1 の設定を使うように適用する
- 3: 1 の設定に以下を読み込ませる
    - scb.hilight
    - 「読み込む対象」は全てをオンにしてください

### マクロの設定
- 以下 3 つのマクロを新規登録し、適当なショートカットキーを設定してください
    - scb_new_or_open.mac
    - scb_swap_line_updir.mac
    - scb_swap_line_downdir.mac

## 使い方
- .scb ファイルを開く
- ゴリゴリ書く
- リンクや行並び替えなどはマクロを使うと便利です

[サンプルファイル](sample/__.scb) も開いてみてください。

## マクロについて
- キーボードショートカットは各自のお好みでどうぞ
- Ctrl + Alt 系は、環境によっては動作しないことが多いようです

### scb_new_or_open.mac
- リンク記法で囲む、リンク先に飛ぶ、URLを開くなど
- 筆者の設定: `Ctrl + Shift + 1`

### scb_swap_line_updir.mac
- 現在行を、一つ上の行と入れ替える
- 筆者の設定: `Ctrl + Shift + k` または `Ctrl + Alt + Up`

### scb_swap_line_downdir.mac
- 現在行を、一つ下の行と入れ替える
- 筆者の設定: `Ctrl + Shift + j` または `Ctrl + Alt + Down`

## 更新履歴
- 2021/01/30 初版

## ライセンス
[MIT](LICENSE)

## 作者
[stakiran](https://github.com/stakiran)
