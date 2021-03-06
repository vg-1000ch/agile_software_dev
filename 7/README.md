# アジャイル設計とは？

## 設計とは
個々で取り上げる設計の意味

### 7.1 ソフトウェアの何が狂うのか？
パス

### 7.2 設計の悪臭 腐敗するソフトウェアの兆候
1. 硬さ
2. もろさ
3. 移植性のなさ
4. 扱いにくさ
5. 不必要な複雑さ
6. 不必要な繰り返し
7. 不透明さ

上記の項目において、今のECナビというシステムだとどんなことがあてはまるだろうか？
詳細 @see p109.


#### 7.2.1 何がソフトウェアを腐敗させてしまうのか？
仕様変更が頻繁に起こるのは既知の事実。仕様変更で設計が劣化していくならば、自分たちの設計に問題がある。プロジェクトが腐敗しないようなプラクティスを導入しなければならない。

#### 7.2.2 アジャイルチームはソフトウェアの腐敗を許さない
各イテレーション時点の要求に最も適した設計(クリーンかつシンプルに保つ)を得るように頑張る。


### 7.3 「コピー」プログラムの例
* 1st Copy
    * Read Keyboard
    * Write Printer
* 2nd Copy
    * Read Keyboard
    * Read Paper Tape(New)
    * Write Printer
* 3rd Copy
    * Read Keyboard
    * Read Paper Tape
    * Write Printer
    * Write Paper Tape(New)

#### 7.3.1 アジャイル設計版のCopyプログラムの例
* Agile Copy
    * Reader
        * Read Keyboard
        * Read Paper Tape
    * Write
        * Write Printer
        * Write Paper Tape(New)

( ﾟ∀ﾟ)o彡OCP！OCP！

#### 7.3.2 アジャイル開発チームは何をすべきかをどうやって知ったのか?
どうやらこのようなステップで見つけたらしい。

1. アジャイルのプラクティスにしたがって問題を発見した。
    * 依存関係逆転の原則(のこと？)
2. 設計の原則を適用して問題を分析した。
3. 適切なデザインパターン(設計パターン,ここではStrategy)を適用して問題を解決した。

※感想 アジャイルアジャイルという単語がでて、私も贖うことの出来ないアジャイルの渦に飲み込まれそうです。

### 7.4 可能な限り美しく設計を保つ
アジャイル開発者はクリーンアップ(可能な限り適切かつクリーンに設計を保つこと)を頻繁に行う。
あとで直すとは決して言わない。

### 7.5 結論
アジャイル設計とは?  
プロセスやイベントではない。原則、パターン、そしてプラクティスを継続的に適用する行為。
※)ソフトウェア設計とパターンは初期段階では過度に対応していない。イテレーションとイテレーションの間で実現している。
