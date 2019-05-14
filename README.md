## 概要

今年度から新しく出来た研究室です．***プログラミング言語の設計および実装***を主な研究テーマとしています．

## メンバー

* 馬谷誠二(准教授)
    * 学位: 博士(情報学)
    * 研究分野: プログラミング言語，言語処理系
    * 担当授業: コンパイラ，情報科学実験II
    * 連絡先: umatani@kangawa-u.ac.jp

## 部屋一覧

* 教員室: 2号館227室(内線2711)
* 学生室: 6号館124室(内線2814)
    * 今のところ誰も使用していません．配属されてくる学生さんの要望を聞きながら，快適な研究環境を整えたいと思っています．

## 研究テーマ

### 分散・協調計算に用いるプログラミング言語

アンビエント計算と呼ばれる分散プロセス計算系をベースに，分散・協調計算のための専用プログラミング言語の開発を行っています．その一つであるSA/Javaは，Safeアンビエントと呼ばれる「場所」と「移動」の概念に基づくプロセス計算を基本モデルとするJava言語用フレームワークであり，高水準な概念に基づいた構造化された並行/分散計算を記述可能となっています．SA/Javaの仕様は，Java言語の諸機能とアンビエントの基本機能である移動動作を互いに干渉することなく統合しています．さらに，アンビエントの移動動作を広域モバイル分散環境上で堅牢に実行するための実装技術にも特徴があります．

また，Java言語以外にLisp言語に対する拡張として実現されているプログラミング環境も開発しています．こちらもSafeアンビエントに基づくプログラミング環境である点は同じですが，SA/Javaとは異なり，動的言語デあるLispの柔軟さを活かしている点が特徴です．たとえば，物理的に分散した複数のプログラマの間での段階的かつインタラクティブなアプリケーション開発などを容易に行うことが可能です．

### 安全性・信頼性を考慮したプログラミング言語

前項のアンビエント計算に基づく分散プログラミング言語の実現のために用いられている各種の協調機能は，より一般のアプリケーションにおけるコンポーネント間の相互作用の安全性の向上を図る目的にも用いることが出来る．

そこで，我々の研究室では，柔軟かつ利便性の高いアクセス制御機能を備えたプログラミング言語の開発を行っています．アンビエント計算に基づく専用の記法によってアプリケーション全体の挙動を制御・管理するのに加え，アクセス制御論理と呼ばれる論理体系に基づく共通インタフェースを介し，汎用プログラミング言語で書かれたコンポーネントとの連携機能も実現することにより，実用的な開発基盤となることを目指しています． 

### 動的言語のためのプログラム解析手法

JVMバイトコードを対象とする静的解析器は数多く存在しますが，それらの解析器は，JavaやScalaのような静的型付き言語からコンパイルされたバイトコード命令列に対しては上手く機能する一方で，動的な言語からコンパイルされたバイトコード命令列に適用すると，ほとんどの解析器は有用な情報を取得することが出来ません．そのような精度の低下の主な原因は，動的言語の動的な振舞いを実現するために用いられる実行時機構の複雑さにあります．

そこで，本研究室では，既存のバイトコードレベルの抽象解釈と呼ばれる手法を用いた動的言語向けの静的解析手法の開発を行っています．我々の手法では，抽象解釈と具象解釈を混ぜながら実行することにより，バイトコードレベルの解析技術に依存しながらも，動的言語の振舞いをある程度正確に把握することが可能となっています．

### 言語処理系開発用ツール

JVMは多様なアプリケーションの実行プラットフォームとして幅広く利用されていますが，特に振舞いの動的な変更を必要とするアプリケーション領域においてバイトコードをクラスロード時に操作する必要があります．そのような処理を実現するためのツールはいくつか存在しますが，多くはJava言語用のライブラリです．しかし，現在，JVMは様々な高水準プログラミング言語の共通プラットフォームであり，バイトコード操作を行うのにJavaに縛られる必要はありません．そこで本研究室では，JVM上で動作するLisp処理系であるClojureのためのバイトコード操作ライブラリを開発しています．本ライブラリは，柔軟な表現能力を備えながら，なおかつ非常に簡潔な記述を特徴としています．具体的には，Lispのマクロのように木として表現されたクラスファイルの一部を，木パターンマッチングと呼ばれる手法を用いて，クラスロード時に書き換えることにより動作します． 

### オブジェクト指向並列言語

Java言語を拡張した高性能並列計算向けのプログラミング言語の開発を行っています．開発している言語の主な特徴としては，細粒度マルチスレッディング，動的fork/join，並列例オ処理，実行時メソッド置換などが挙げられます．また，言語の設計だけではなく，細粒度マルチスレッディングを実現するための効率良い実装手法の構築や，並列例外処理機構の開発なども行っています． 

## ゼミについて

3年生後期の情報ゼミナールでは：

* 言語処理系の中身を理解する
* 自分の知らないプログラミング言語を新たに一つ習得する

ことを目標に，2冊程度の書籍の輪講を行う予定です．どちらも，具体的にどのプログラミング言語を対象とするかによって選ぶ書籍は異なります．4年生に進んでからの本研究室での研究に活用でき，かつ，習得した知識を社会に出てからも幅広く活用できるような(なるべく)モダンなプログラミング言語を，こちらからいくつかお勧めするつもりです．具体的には：

* Haskell
* OCaml
* Scala
* Clojure
* Scheme
* TypeScript

あたりを今のところ検討中てす．

また，研究を進めるにあたり英語で書かれた文献の読解は必須スキルですので，上記輪講の少なくとも1冊は洋書にし，英語読解能力を鍛えてもらうつもりです．
