# 量子コンピュータアート2025

## 自然と計算、計算と芸術

古典計算は、チューリングマシンという抽象機械によってモデル化され、離散的かつ確定的な古典ビットで表現される決定論的な数を操作することで計算を進めていく。

それに対して量子ビットと量子回路によってモデル化される量子計算は、量子という自然現象そのものを情報処理システムとして捉え、そのメカニズムを直接用いて計算を行う自然計算である。

量子計算は、「自然そのものを用いて行われる計算」であり、古典計算を用いて自然をシミュレートするのではなく、自然現象をそのまま計算として用いようとする点にその本質がある。

そうした観点からは、量子コンピュータアートを「自然計算芸術」として位置付けることができる。

## 量子計算

古典コンピュータの情報の最小単位であるビットは0または1のいずれかの値を取り、これらを組み合わせて整数や実数など、私たちが普段使う数を表現し、計算を行っていた。

量子コンピュータの情報の基本単位、すなわち量子コンピュータにおける「数」は量子ビット $|\psi⟩$ という2次元ベクトルである。それは、$|0⟩$ と $|1⟩$ という明確に区別された二つの「計算基底」の線形結合で表される。

$|\psi⟩ = \alpha|0⟩ + \beta|1⟩$ ただし $|\alpha|^2 + |\beta|^2 = 1$

ここで、2つの係数 $\alpha$ と $\beta$ が複素数であることが重要である。これらが複素数であることで、量子ビットがアナログな連続量をとるベクトルであるという
だけでなく、「位相」という情報も持つことで、量子コンピュータ独自の数と計算の概念をつくりだす。


# 量子コンピュータアート

こうした量子計算と計算を実行する量子コンピュータそのものに目を向けることで、新たな芸術表現を生み出すことができないか？

## 「見えないもの」と「見えるもの」

量子コンピュータアートに対するアプローチを、「見えないもの」と「見えるもの」の2つの軸で考える。

見えないものは、量子状態を表す状態ベクトルや密度行列であり、それらは複素数のベクトルや行列で表される。

見えるものは、量子状態の測定結果と量子コンピュータの実機そのものである。

見えないものは抽象的だが、一般的であり量子コンピュータアートの共通素材である。

見えるものは具体的、個別的、物理的であり、さまざまな試行錯誤が現在進行中である。


![見えないものと見えるもの](https://paper-attachments.dropboxusercontent.com/s_2D91BCD458DE61F6535938CCADF8F5619DD515D7B62CCEBA4F3999A1EA268D1B_1745993790697_overview.jpg)



## 見えないもの

### 量子情報芸術

- 状態ベクトルと密度行列の美学を探求する。美的な状態ベクトル、美的な密度行列とはどのようなものか？
- 量子プログラミングを通じて美的な量子状態を探求する。
- 量子情報理論によって情報美学を量子情報美学に拡張する。

### 量子コンピュータの情報構造

量子コンピュータは、量子状態にある物質を使って行うアナログ計算である。$n$個の古典ビットが、$2^n$通りの異なる数しか表現できないのに対して、量子計算は連続的な複素数の集まり（複素ヒルベルト空間）によって行われる。


![量子コンピュータの情報構造](https://paper-attachments.dropboxusercontent.com/s_6C777791E4F46067E274070DF10B84E76C3E66AA459DA8F5CF900E3B5F08ED3F_1742479947112_infostructure.png)


表1：量子ビット数と状態ベクトル、密度行列の自由度

| 量子ビット数 | 状態ベクトルのサイズ  | 状態ベクトルの自由度               | 密度行列のサイズ                   | 密度行列の自由度                   |
| ------ | ----------- | ------------------------ | -------------------------- | -------------------------- |
| $1$  | $2$       | $2^2 - 2 = 2$          | $2 \times 2$             | $2^2-1=3$                |
| $2$  | 4           | $2^3 - 2 = 6$          | $4 \times 4$             | $2^4-1=15$               |
| $3$  | $8$       | $2^4 - 2 = 14$         | $8 \times 8$             | $2^6-1=63$               |
| $4$  | $16$      | $2^5 - 2 = 30$         | $16 \times 16$           | $2^8-1=255$              |
| $5$  | $32$      | $2^6 - 2 = 62$         | $32 \times 32$           | $2^{10}-1=1023$          |
| $8$  | $256$     | $2^9 - 2 = 510$        | $256 \times 256$         | $2^{16}-1=65535$         |
| $10$ | $1024$    | $2^{11} - 2 = 2046$    | $1024 \times 1024$       | $2^{20}-1=1048575$       |
| $20$ | $1048576$ | $2^{21} - 2 = 2097150$ | $1048576 \times 1048576$ | $2^{40}-1=1099511627775$ |


量子ビットの数が増えていくにしたがって、その自由度は急激に増加する。



### [Quantumf*uck](https://github.com/hemokosa/quantumfuck)：詩的量子プログラミング言語

Quantumf*ckは、難解（[Esoteric](https://esolangs.org/wiki/Main_Page)）プログラミング言語の [brainf*ck](https://esolangs.org/wiki/Brainfuck) と、詩的（Poetic）プログラミング言語の [Coem](https://www.coem-lang.org/) を参考に、最小の記述量で多様な量子回路を柔軟に記述できることを目指している。

Quantumf*ckは [Python](https://www.python.org/) とさまざまな量子コンピュータやシミュレータ上で量子アルゴリズムを作成、実行するためのオープンソースライブラリの [quri-parts](https://quri-parts.qunasys.com/) を用いて実装されている。


#### Quantumf*ckのコマンド一覧
| 命令   | 量子回路操作                                      |
| ---- | ------------------------------------------- |
| >    | 次の量子ビットを操作対象にする（ポインタを+1）                    |
| <    | 前の量子ビットを操作対象にする（ポインタを-1）                    |
| +, H | Hadamardゲートを適用                              |
| ~, T | $\pi / 4$位相シフトゲートを適用                      |
| x, X | Pauli-X（ビット反転）ゲートを適用                      |
| @, C | CNOTゲートを適用（Targetは次の量子ビット、あるいは続く数字で指定する）    |
| :    | 測定値を状態ベクトルから推定（実際に測定は行わない）                  |
| ,    | 状態ベクトルの初期化                                  |
| ;    | 状態ベクトルのランダマイズ                               |
| [    | ループ開始                                       |
| ]    | 条件付きループ終了（測定値が0の場合はループを抜ける、それ以外はループの先頭に戻る）  |
| ?    | Hadamardゲート、あるいは$\pi / 4$位相シフトゲートをランダムに適用 |
| !    | 操作対象の量子ビット（ポインター）をランダムに移動                   |
| *    | 実行箇所をランダムに移動                                |

- 使用できる量子ゲートは、万能量子ゲート（任意の量子演算を近似可能な量子ゲートの最小構成）である「Hadamardゲート」「$\pi / 4$位相シフトゲート」「CNOTゲート」の組のみとする。

表の最後の3つのコマンドは回路と実行に偶然性を与えるためのものである。加えて、実行時に「regex」フラグをTrueにすることで、コードを[正規表現](https://angelhousepress.com/essays/waber-regular-expressions-as-a-system-of-poetic-notation-plus-bio.pdf)として解釈し、それに一致する文字列を生成して実行する（[Exrex](https://pypi.org/project/exrex/)ライブラリを使用）。そうすることで、制御構造を記述し、コード自体にも偶然性や多義性を導入することができる。

- Quantumf*ck：https://github.com/hemokosa/quantumfuck


## Hello, quantum!: +@


    # クラスのインスタンス化
    num = 2
    qf = QF(num, regex=False, debug=True)
    # コードを実行
    code = "+@"
    state, history, command, circuit = qf.parse(code)
    # 状態ベクトルの履歴を出力
    for i, s in enumerate(history):
        print(f"Step {i}: {s.get_vector()}")
    # 回路の可視化
    circuit_drawer(circuit, "mpl")


    (0, 0): Command: +, Pointer: 0
    (1, 1): Command: @, Pointer: 0
    Quantum Circuit Execution Completed
    Step 0: [0.70710678+0.j 0.70710678+0.j 0.        +0.j 0.        +0.j]
    Step 1: [0.70710678+0.j 0.        +0.j 0.        +0.j 0.70710678+0.j]
![](https://paper-attachments.dropboxusercontent.com/s_7B7A7D49FB065DFAD7738D4F1FF9D31312B12BB125A1683AF03583C3352FFDB4_1736176083683_file.png)

    # サンプリング（全量子ビットを測定）
    shots = 20
    samples = state.sampling(shots)
    print("Sampling Results:", samples)
    print([format(value, "b").zfill(num) for value in samples])


    Sampling Results: [3, 3, 0, 0, 0, 3, 3, 0, 0, 3, 0, 3, 3, 3, 3, 3, 3, 0, 0, 3]
    ['11', '11', '00', '00', '00', '11', '11', '00', '00', '11', '00', '11', '11', '11', '11', '11', '11', '00', '00', '11']


---


## 複素数によるデザイン(Design by Complex Numbers)

量子計算のポイントは、それが複素数によって記述され、複素数によって操作されるということにある。実数が、1 本の数直線上の「点」として表される一次元の数であるのに対し、複素数は、実部と虚部の線型結合からなる二次元のベクトルである。


## 複素数のイメージスキーマ

実数は、「経路（Path）」というイメージスキーマを中心に、大小や順序、移動や伸縮といった数直線上の位置や動きによって、数や演算が身体化されている。

それに対して複素数のイメージスキーマは、数直線から複素平面という「空間」のスキーマに加えて「平面上に点を置き、その点を伸縮したり回転する」という「ベクトル（VECTOR）」「回転（ROTATION）」「スケール（SCALING）」というスキーマが複雑に組み合わさったものとなっている。

この中でも特に重要なものが「回転」である。回転のスキーマは、複素数の乗算という具体的な演算に対応しているだけでなく、円運動や螺旋などの豊かな視覚イメージを生み出す共通言語でもある。

## 回転を体得する

虚数単位 $i$ の導入が、一次元の実数の世界から2次元の複素平面への拡張を生み出し、「回転」という新たな幾何学的操作を概念化することで、複素数の豊穣な構造が生み出された。

しかし複素数は、単なる数学的な抽象概念ではない。複素数は、回転を簡潔に表現するための優れたデザインツールでもある。美的な量子状態をデザインするためには、この回転を視覚的、身体的に体得し、回路設計に活用することが、必要不可欠となる。

複素平面上での回転は、複素数の掛け算として表現できる。この性質は、量子力学における波動性を表現する際に、特に有用である。複素数と聞くと、一瞬難解に感じてしまうかもしれないが、複素数をその形式だけでなく、視覚的、身体的に捉えることは、量子力学に限らず私たちの周りの世界をより深く理解することにつながる。

量子の状態は複素ベクトルで表現され、量子の状態の変化は、複素行列との積で表現される。


### 複素数を操作してみる

https://editor.p5js.org/hemokosa/sketches/focuNSu84

これは p5.js を使って 2成分の複素ベクトル（単一量子ビットの状態ベクトル）を画面上に可視化し、インタラクティブに操作できるスケッチである。

- 画面下部の入力欄で、状態ベクトルの成分やスカラー・行列要素を数値入力できる
- 対応するボタンを押すと、即座に画面中央の矢印に反映される
- 「正規化」で長さを 1 に揃えたり、「リセット」で初期状態に戻したりできる

1量子ビットの状態操作やユニタリー変換、スカラー変換の効果を視覚的に確かめることができる。

### 複素数は波である

虚数単位 $i$ は「位相を回転させながら確率振幅を保存する」ための装置であり、これが量子を「波（振動）」として振る舞わせる。複素ベクトルという矢印の長さが測定でしかわからず、向きは干渉でしかわからないことが、量子の粒子と波動の「二重性」を表現している。位相は波動性を表現するためには必須の自由度である。

つまり、複素数は「見えない振動」を内部に抱えた確率のキャリアであり、その振動があるからこそ量子は波として振る舞うと同時に、測定することで離散的な粒となる。

複素数で表現される測定前の量子状態は、大きさと位相を持つ波であり、それを測定することによって、大きさだけが統計的に残る粒子となる。波から粒への変化は、この位相の消去によって起こる。逆にいえば、量子状態が複素数で表現されている限り、量子はいつでも波動でもあり粒子でもある。

https://editor.p5js.org/hemokosa/sketches/3BOA_r19U

これは p5.js を使って 2量子ビットの状態ベクトル（複素振幅と位相）を波として可視化し、インタラクティブに操作できるスケッチである。また、簡易的な量子ゲート操作とエンタングルメントの指標（コンカレンス）を示すスケッチである。

- 量子ビットの状態ベクトル を複素振幅・位相スライダーで編集
- 単1/2量子ビットゲート をリアルタイムで適用
- 正規化とスライダー同期で常に正規化される
- 波形描画で振幅・位相の時間的変化を可視化
- コンカレンス計算でエンタングルメントの強さを数値表示

2量子ビットの量子回路の基本的な挙動を、視覚的かつインタラクティブに確かめることができる。


## 3量子ビットベンチマーク回路

シンプルな3量子ビットの回路で、状態ベクトルと密度行列の複素数の挙動を見てみる。

同時にこの回路は、阪大QIQBの実機で継続的に実行する、量子コンピュータの性能向上のベンチマーク回路としても用いる。

## [Quantumf*ck](https://github.com/hemokosa/Quantumfuck)
## (H>){3}(T>){3}C>C>>T>>HC>H>>T>C2


    # Instantiate class
    num = 3
    qf = QF(num, regex=True, debug=True)
    # Execute code
    code = "(H>){3}(T>){3}C>C>>T>>HC>H>>T>C2"
    state, history, command, circuit = qf.parse(code)


![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745570282510_Screenshot+2025-04-24+at+11.57.45.png)



    Code: H>H>H>T>T>T>C>C>>T>>HC>H>>T>C2
    (0, 0): Command: H, Pointer: 0
    (1, 1): Command: >, Pointer: 0
    (2, 1): Command: H, Pointer: 1
    (3, 2): Command: >, Pointer: 1
    (4, 2): Command: H, Pointer: 2
    (5, 3): Command: >, Pointer: 2
    (6, 3): Command: T, Pointer: 0
    (7, 4): Command: >, Pointer: 0
    (8, 4): Command: T, Pointer: 1
    (9, 5): Command: >, Pointer: 1
    (10, 5): Command: T, Pointer: 2
    (11, 6): Command: >, Pointer: 2
    (12, 6): Command: C, Pointer: 0
    (13, 7): Command: >, Pointer: 0
    (14, 7): Command: C, Pointer: 1
    (15, 8): Command: >, Pointer: 1
    (16, 8): Command: >, Pointer: 2
    (17, 8): Command: T, Pointer: 0
    (18, 9): Command: >, Pointer: 0
    (19, 9): Command: >, Pointer: 1
    (20, 9): Command: H, Pointer: 2
    (21, 10): Command: C, Pointer: 2
    (22, 11): Command: >, Pointer: 2
    (23, 11): Command: H, Pointer: 0
    (24, 12): Command: >, Pointer: 0
    (25, 12): Command: >, Pointer: 1
    (26, 12): Command: T, Pointer: 2
    (27, 13): Command: >, Pointer: 2
    (28, 13): Command: C, Pointer: 0
    Quantum Circuit Execution Completed



# Quantum Visual Systems

## 点・線・面から、複素平面（ベクトル）のパッチワークへ

複素数のベクトルによって体系的に表現される量子状態を視覚化するためには、点・線・面という古典的な幾何学の要素による思考から、複素平面上を移動、伸縮、回転する線分を空間に埋め込んでいく、複素平面のパッチワークという思考が有効である。


## 状態ベクトルのダンス


- 習作1：一列に並べる
![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745586456792_animation.gif)

![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745586635713_file.png)


- 習作2：重ねる

![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745670513924_file.png)

![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745670578809_state_ring.gif)

- 習作3：連結する

![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745586564804_state_smooth_history.gif)

![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745586660740_file.png)


- 習作4：色にマッピング（振幅→明度・位相→色相）

横方向
![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745586693499_file.png)

縦方向
![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745586682840_file.png)

- 習作5：形にマッピング（振幅→明度・位相→傾き）

![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745589437288_file.png)


- 習作6：連続的に表示する（スペクトル）

![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745589899284_quantum_stripes_animation.gif)

![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745589242655_file.png)


## 密度行列の風景


- 習作7：グリッド状に配置して45度傾ける

![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745586786061_density_animation.gif)

![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745586883668_file.png)


- 習作8：色にマッピング（振幅→明度・位相→色相）

![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745586927070_density_color.gif)

![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745586951418_file.png)

![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745586968349_file.png)


- 習作9：ベクトルによるグリッドの変形

![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745589725528_density_grid.gif)

![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745589680440_file.png)



## 美的測度（量子情報美学）

QVSによって表現された量子状態の美学を探求していくためには、どうしたらいいのだろうか。それをただ既存の美的体験に照らし合わせて評価しただけでは、量子状態に内在する位相やエンタングルメントといった重要な特徴を考慮することができない。

そこで、量子状態の美学を数値的に探索するための美的測度を提案する。ジョージ・D・バーコフからマックス・ベンゼの情報美学を参考に、以下の4つの指標を用いて美的測度を定義することを試みる。

- 秩序（$O$）：振幅と位相の周期自己相関の和
- 複雑性（$C$）：振幅エントロピーと位相エントロピーの和（複素エントロピー）
- 量子的不確実性（$QU$）：各量子ビットのエンタングルメント・エントロピーの和
- 古典的不確実性（$CU$）：各量子ビットの測定における確率分布のシャノン・エントロピー

ここで「秩序」と「複雑性」は、従来の古典情報美学の考え方を、複素数の振幅と位相それぞれに適用したものである。

そこに「不確実性」を導入することで、量子状態固有の特徴を考慮する。不確実性は、量子状態特有のエンタングルメントによる「量子的不確実性」と、測定結果の確率分布による「古典的不確実性」の双方を考慮する。

量子状態の美的測度は、以下のように、これら4つの指標の幾何学的平均として求めることにする。

**美的測度**（$M$）：$M = \sqrt[4]{O \times C \times QU \times CU}$

美的測度は、それがそのまま対象の美を現すものではないが、美的な量子状態を探索していくための補助線として活用していきたい。


- ジョージ・D・バーコフ (George D. Birkhoff) – Aesthetic Measure (1933)：美を秩序と複雑性で定式化した先駆者 ￼。提案モデルは M = O / C 。


- ハンス・J・アイゼンク (H. J. Eysenck) – “The Empirical Determination of an Aesthetic Formula” (1941)：バーコフの測度を検証し、M = O × Cという美の公式を提案。


- エイブラハム・モールズ (Abraham Moles) – Information Theory and Esthetic Perception (1958)：情報理論に基づく美学を展開し、バーコフの公式の代替案として M = O × C を示唆 ￼。複雑さと秩序の情報量で美を計量化する「情報美学」の基礎を築いた。


- マックス・ベンゼ (Max Bense) – Aesthetica 全4巻 (1954–1960): ドイツにおける情報美学の開拓者。バーコフのアイデアにシャノンの情報理論を統合し、美を数理的に論じた。Benseは「美的情報」という概念を初めて使用し ￼、美学を秩序と情報量の問題として捉え直した。


## 美的測度の事例

![](https://paper-attachments.dropboxusercontent.com/s_2D91BCD458DE61F6535938CCADF8F5619DD515D7B62CCEBA4F3999A1EA268D1B_1745743059886_file.png)

- 0〜2ステップ：Hゲートで最大限の重ね合わせを作る（複雑性と古典的不確定性の増加）。
- 3〜5ステップ：Tゲートにより状態ベクトルに位相干渉を起こす（複雑性の増加）。
- 6〜7ステップ：CNOTゲートでエンタングルメントを生成（量子的不確定性の増加）。
- 8〜9ステップ：T, Hゲートで振幅を変化させる（複雑性の増加と秩序の低下）。
- 10〜13ステップ：さらなる振幅と位相の変化をおこす（不確定性の増加）。

5〜10ステップの状態ベクトル（8ステップ目が美的測度の最大値）

![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745574578528_file.png)

10〜13ステップの状態ベクトル

![](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745574675118_file.png)


## 美的な量子状態のデザイン技法

量子状態の「秩序」「複雑性」「不確定性」をバランス良く最大化するにはどうすればいいか？

層構造を構成的に組み合わせる

- 重ね合わせの最大化（Hゲート）
- 位相による複雑化（Tゲート）
- エンタングルメントの生成（CNOTゲート）

量子状態の規則性とランダム性のバランス

- 重ね合わせとエンタングルメントの規則的構造に位相を注入する
- ランダムな重ね合わせと位相をエンタングルメントさせる

回路自体（量子ビットレベル）における反復や対称性（秩序）の導入

既存の量子アルゴリズムの簡略化

- 量子ウォーク/量子カオス
- 量子位相推定（Shorのアルゴリズム）
- 量子フーリエ変換
- オラクル回路（Groverのアルゴリズム）

---


### より多数の量子ビットの美的回路の例を載せる

---


# 見えるもの


## 実機による実行：統計詩学

- 確率分布としての詩的構造
- マクロ（確率）とミクロ（宿命）（統計性と一回性）
- ノイズの詩学







## サンプリング例（X測定、Y測定、Z測定）
![X軸、Y軸、Z軸それぞれでの測定](https://paper-attachments.dropboxusercontent.com/s_C785E01A970B1C64484F9DAFFDB9A61AC1C230A508A9F549281A7878D15AA124_1745759595644_file.png)


## 阪大実機による3量子ビットGHZ回路の実行（2025.04.22）

![](https://paper-attachments.dropboxusercontent.com/s_2D91BCD458DE61F6535938CCADF8F5619DD515D7B62CCEBA4F3999A1EA268D1B_1745591419284_Screenshot+2025-04-25+at+23.29.37.png)


![](https://paper-attachments.dropboxusercontent.com/s_6C777791E4F46067E274070DF10B84E76C3E66AA459DA8F5CF900E3B5F08ED3F_1745455831223_Screenshot+2025-04-22+at+10.08.49.png)

| **ジョブID**     | 06806ea3-0676-71dc-8000-8701ce90c0be |
| ------------- | ------------------------------------ |
| **ジョブ名**      |                                      |
| **説明**        |                                      |
| **ジョブタイプ**    | sampling                             |
| **デバイスID**    | anemone                              |
| **ショット数**     | 1024                                 |
| **ステータス**     | succeeded                            |
| **Submit 日時** | 2025-04-22T01:00:32Z                 |
| **Ready 日時**  | 2025-04-22T01:00:36Z                 |
| **実行日時**      | 2025-04-22T01:00:36Z                 |
| **終了日時**      | 2025-04-22T01:00:37Z                 |
| **実行時間 (秒)**  | 1.043                                |
| **メッセージ**     | job is succeeded                     |



    {
      "name": "",
      "description": "",
      "shots": 1024,
      "deviceId": "anemone",
      "jobType": "sampling",
      "jobInfo": {
        "program": [
          "OPENQASM 3;\ninclude \"stdgates.inc\";\nqubit[3] q;\nbit[3] c;\n\nh q[0];\ncx q[0], q[1];\ncx q[0], q[2];\nc = measure q;"
        ],
        "combined_program": "",
        "operator": null,
        "result": {
          "sampling": {
            "counts": {
              "101": 20,
              "110": 54,
              "111": 398,
              "010": 38,
              "001": 34,
              "000": 478
            },
            "divided_counts": null
          },
          "estimation": null
        },
        "transpile_result": {
          "transpiled_program": "OPENQASM 3.0;\ninclude \"stdgates.inc\";\nbit[3] c;\nrz(pi/2) $0;\nsx $0;\nrz(pi/2) $0;\nrz(pi/2) $2;\nsx $2;\nrz(pi/2) $2;\ncx $2, $1;\ncx $0, $1;\nrz(pi/2) $0;\nsx $0;\nrz(pi/2) $0;\nrz(pi/2) $1;\nsx $1;\nrz(pi/2) $1;\nrz(pi/2) $2;\nsx $2;\nrz(pi/2) $2;\nc[0] = measure $1;\nc[1] = measure $2;\nc[2] = measure $0;\n",
          "stats": {
            "before": {
              "n_qubits": 3,
              "n_gates": 6,
              "n_gates_1q": 4,
              "n_gates_2q": 2,
              "depth": 4
            },
            "after": {
              "n_qubits": 3,
              "n_gates": 20,
              "n_gates_1q": 18,
              "n_gates_2q": 2,
              "depth": 9
            }
          },
          "virtual_physical_mapping": {
            "0": 1,
            "1": 2,
            "2": 0
          }
        },
        "message": "job is succeeded"
      },
      "transpilerInfo": {
        "transpiler_lib": "qiskit",
        "transpiler_options": {
          "optimization_level": 1
        }
      },
      "simulatorInfo": {},
      "mitigationInfo": {
        "ro_error_mitigation": "pseudo_inverse"
      }
    }


![](https://paper-attachments.dropboxusercontent.com/s_6C777791E4F46067E274070DF10B84E76C3E66AA459DA8F5CF900E3B5F08ED3F_1745456993334_Lines250422.png)

![](https://paper-attachments.dropboxusercontent.com/s_6C777791E4F46067E274070DF10B84E76C3E66AA459DA8F5CF900E3B5F08ED3F_1745457002788_Kanji250422.png)




# 量子コンピュータのライフログ
## QBMP（量子ビットマップフォーマット）を大阪大学と共同開発中


- チップの状態と操作の記録＋日時＋測定結果＋コメント＝記録日記
- 自然計算の記録から量子コンピュータ気象学へ


![](https://paper-attachments.dropboxusercontent.com/s_2D91BCD458DE61F6535938CCADF8F5619DD515D7B62CCEBA4F3999A1EA268D1B_1745730616123_.jpg)

![](https://paper-attachments.dropboxusercontent.com/s_6C777791E4F46067E274070DF10B84E76C3E66AA459DA8F5CF900E3B5F08ED3F_1744895271393_20250331.jpg)

![](https://paper-attachments.dropboxusercontent.com/s_6C777791E4F46067E274070DF10B84E76C3E66AA459DA8F5CF900E3B5F08ED3F_1742222810743_image.png)

![Qubit周波数](https://paper-attachments.dropboxusercontent.com/s_6C777791E4F46067E274070DF10B84E76C3E66AA459DA8F5CF900E3B5F08ED3F_1744894782376_qubit_frequency.png)

![ベル状態（エンタングルメント）とX90忠実度](https://paper-attachments.dropboxusercontent.com/s_6C777791E4F46067E274070DF10B84E76C3E66AA459DA8F5CF900E3B5F08ED3F_1744894795084_bell_distribution.png)

# 統計詩学（Statistic Poetics）

統計力学の概念は一見すると詩や文学とは無縁に思えるが、20世紀以降、多くの詩人や批評家が確率、無秩序と秩序、エントロピー、自己組織化といった概念を創作論や文学理論に取り入れてきた。とりわけ今日の詩学では、エントロピーは「現代世界が冗長性や無統一に向かう傾向を示す重要なメタファー」とまで言われている。


## ミクロ美学とマクロ美学（マックス・ベンゼ）

ミクロ美学：細部や部分的な要素に注目する美的分析

- 局所的なディテールや小さな構造的要素を扱う。
- ローカルなエントロピーや秩序、それらと全体の関係を評価する。
- 精緻な技術や素材感、微細な変化に美的価値を見出す。

マクロ美学：作品全体の構造や大きな枠組みに焦点を当てた美的分析

- 全体的な印象や大規模なパターンを扱う。
- 作品全体のエントロピー（情報量）や秩序、バランスを評価する。
- 視覚的・概念的・構造的な全体像にもとづいた美的価値を考える。


## ミクロ詩学とマクロ詩学

ミクロ詩学：測定結果の各ショットに着目する。

- 宿命（Desitiny）：一回性の詩学、いかなる結果も引き受ける
- 消失（Vanishment）：測定の不可逆性、収縮と分岐
- 最小（Minimum）：ショットの詩学、ビット列の音律
- 時刻（Timestamp）：記録とアーカイヴ、クロノポエティクス

マクロ詩学：多数の測定結果の統計的分布に着目する

- 堆積（Accumulation）：多数の測定から現れる構造
- 消尽（Epuise/Exhausted）：可能性を汲み尽くす
- 沈黙（Silence）：現れない結果、物理的否定
- 復元（Restore）：読解による可逆性の出現



## 量子コンピュータアート


![量子コンピュータアート](https://paper-attachments.dropboxusercontent.com/s_6C777791E4F46067E274070DF10B84E76C3E66AA459DA8F5CF900E3B5F08ED3F_1742394163319_Quantum+Computer+Art+2.png)


## インターフェイスとしての量子ビット

量子ビットや量子回路、測定結果は、量子コンピュータアートの直接的な対象ではない。量子コンピュータアートの中心的対象は、量子チップ上で物理的に実現している量子状態そのものである。

量子ビットや量子回路、測定結果は、量子状態という見えない対象と、私たちを含めて古典状態にある世界とのインターフェイスである。


![見えるものと見えないもの](https://paper-attachments.dropboxusercontent.com/s_2D91BCD458DE61F6535938CCADF8F5619DD515D7B62CCEBA4F3999A1EA268D1B_1745728694694_Screenshot+2025-04-27+at+12.23.02.png)


## 付録：「量子を待ちながら」Generative Manga（試作）

（状態ベクトルの木を挟んで2人の人が会話をするマンガをつくりたい）

![](https://paper-attachments.dropboxusercontent.com/s_6C777791E4F46067E274070DF10B84E76C3E66AA459DA8F5CF900E3B5F08ED3F_1744896743778_Quantum_Godot_comic-20250416-225733.png)


Paul Tolliver Brown, “[Quantum Theory and Samuel Beckett’s Endgame.](https://www.literatureandscience.org/wp-content/uploads/2022/10/15.1-Pathak-on-Brown.pdf)” Configurations 29. 3 (2021): 241 – 265.
