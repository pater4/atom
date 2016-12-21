## 設定のインストール
Mac環境での説明です。   
Windowsの場合は若干調整が必要です。
```
mv ~/.atom ~/.atom_bak
git clone https://t_sakuma@bitbucket.org/t_sakuma/atom.git ~/.atom
```

## パッケージのインストール
`apm install --packages-file ~/.atom/atom-packages.txt`

## config.csonの設定
以下のパスを環境に合わせて変更
```
    projectHome: "/Users/t.sakuma"
```
```
"linter-phpmd":
    executablePath: "/Users/t.sakuma/.composer/vendor/bin/phpmd"
    rulesets: "/Users/t.sakuma/.atom/ruleset.xml"
```
## 背景画像の変更
- editor-backgroundパッケージの設定で変更可能
- シェル画面の背景変更はstyles.lessの35行目あたりのURLを変更

## キー設定
基本はvim-modeとその他プラグインの設定をそのまま使っているが以下の変更をしている
- Altキー押しながらhjklで矩形選択
- `space m`でハイライト、`space M`で解除
- `ctrl-k`で入力モード解除
- 編集モード時`ctrl-j`で保存

## シェル
terminal-plusはデフォルトでzshが選択されている

## UML図
色々設定が面倒なので必要ないならplantuml-viewerをアンインストール

## UI
基本タブ移動はしないので非アクティブのタブは非表示

## よく使うショートカットキー
### エディタ操作
vimの基本操作は除く

|キー  |説明  |使用頻度|
|------|------|------|
|ctrl-k|入力モード解除|★★★|
|ctrl-j|保存|★★★|
|cmd-b|バッファ移動|★★★|
|ctrl-`|シェル画面を開く|★★★|
|cmd-p|ファイル移動|★★|
|cmd-f|ファイル内検索|★★|
|cmd-F|プロジェクト内検索|★★|
|space m|ハイライト|★★|
|shift-enter|簡易移動|★★|
|ctrl-alt-t|差分確認|★★|
|ctrl-alt-[n or p]|差分箇所に移動|★★|
|cmd-P|コマンド入力|★|
|ctrl-,|Atom設定画面を開く|★|
|ctrl-M|マークダウン表示|★|

### ファイルツリー操作
|キー  |説明  |使用頻度|
|------|------|------|
|ctrl-0|ファイルツリーに移動|★★|
|ctrl-&#124;|現在のファイルを元にファイルツリーに移動|★★|
|h or j or k or l|移動|★★|
|esc|ファイルツリーから抜ける|★|
|a|ファイル追加|★|
|A|ディレクトリ追加|★|
|d|ファイル複製|★|
|m|ファイル移動|★|
|delete|ファイル削除|★|
