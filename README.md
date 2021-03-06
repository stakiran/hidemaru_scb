# hidemaru_scb
秀丸エディタでScrapbox風味の記法やリンクを実現する

![image](https://user-images.githubusercontent.com/23325839/106346071-bea72000-62f7-11eb-97bd-472eb61ea312.png)

## ダウンロード
- [Releaseページ](https://github.com/stakiran/hidemaru_scb/releases) よりダウンロードできます

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
- 2021/03/17
    - fix scb_new_or_open.mac利用時に検索ダイアログの設定が乱れる問題
        - 現在の設定を保存しておき、処理後に復元する処理を追加することで回避
    - fix 引用の強調表示がされないケース
    - fix 1文字のインデント無し行がアウトラインされない
- 2021/01/30 初版

## ライセンス
[MIT](LICENSE)

## 作者
[stakiran](https://github.com/stakiran)
