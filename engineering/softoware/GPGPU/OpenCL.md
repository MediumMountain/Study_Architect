# OpenCL
- 様々なデバイスで使えるプログラム言語であり、GPUを活用した並列計算を行うために使われます。
- OpenCLを使用することで、CPUのみを使用する場合よりも高速に処理を行うことができます

OpenCL（Open Computing Language）は、CPU（Central Processing Unit）、GPU（Graphics Processing Unit）、DSP（Digital Signal Processor）、FPGA（Field Programmable Gate Array）などで構成される異種混在環境（ヘテロジニアス・システム）で並列処理を使用するプログラムを作成するためのフレームワークで、オープンかつロイヤルティー・フリーの標準規格です。標準 ANSI C (C99) をベースとしたプログラミング言語で、ソフトウェア開発者が様々なプラットフォームに対しパフォーマンス向上をもたらすことのできるプログラミング・モデルです。2008年6月に米アップルが発表したのち、現在は米クロノス・グループがAPIの策定を行っています。

OpenCLでは、ホスト（CPU）とデバイス（GPU）があります。ホスト側でOpenCLプログラムを作成し、デバイスに処理を割り当てます。そして、デバイス上で並列処理を行い、結果をホストに返します。

OpenCLのプログラムは、次のような構成になっています。

1. プラットフォームの選択
2. デバイスの選択
3. コンテキストの作成
4. プログラムの作成とコンパイル
5. カーネルの作成
6. キューの作成
7. データの転送
8. カーネルの実行
9. 結果の取得




https://www.fu.is.saga-u.ac.jp/yaman/OPENGLCL/openglcl.pdf