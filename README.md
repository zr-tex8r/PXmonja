PXmonja パッケージバンドル
==========================

LaTeX： (u)pLaTeX において日本語を等幅で組む

PXmonja パッケージは、端末表示を模したいわゆる「等幅」出力、すなわち 「欧文を和文の半分の幅にしてベタ組」する機能を提供する。 Verbatim 出力でもそれ以外でも使用可能である。 

### 前提環境

  - TeX 処理系： pLaTeX2e / upLaTeX2e
  - DVI ウェア： dvipdfmx

### 本ソフトウェアの作者のサイト

  - En toi Pythmeni tes TeXnopoleos ～電脳世界の奥底にて～  
    <http://zrbabbler.sp.land.to/>

  - 以下のページに一部機能の使用例を紹介した。  
    「PXmonja パッケージ」  
    <http://zrbabbler.sp.land.to/pxmonja.html>

### インストール

  - TDS 1.1 に従ったシステムでは、各ファイルを次の場所に移動する。
      * `*.sty`   → $TEXMF/tex/platex/pxmonja/
      * `*.sfd`   → $TEXMF/fonts/sfd/pxmonja
      * `*.tfm`   → $TEXMF/fonts/tfm/public/pxmonja
      * `*.vf`    → $TEXMF/fonts/vf/public/pxmonja
      * `pdfm-pxmonja.map` → $TEXMF/fonts/map/dvipdfmx/pxmonja

  - W32TeX を `C:\usr\local` にインストールした場合(☆)は、
    上の記述の $TEXMF を `C:\usr\local\share\texmf-local`
    としパス区切りの `/` を `\` に変更したディレクトリとなる。
    (必要に応じて mktexlsr を実行する。)

#### フォントマップ登録(dvipdfmx)

dvipdfmx の設定ファイル dvipdfmx.cfg に次の行を追加する。

    f pdfm-pxmonja.map

※ (☆)の場合、設定ファイルは以下の場所にある。

    C:\usr\local\share\texmf\dvipdfmx\config\dvipdfmx.cfg

※ このパッケージではパッケージ読込時のオプション `font`
によりフォントを指定できる。
常に `font` 指定を行うであれば、この作業は不要である。

#### フォントマップ登録(dviout)

パッケージ中の dviout-pxmonja.map が dviout 用のマップファイルである。
(登録の手順の詳細は省略する。)

pxmonja パッケージ (v0.2) -- 本体
---------------------------------

まだ解説が書けておりません…。
基本的な機能の説明については以下の Web ページで行っていますので、
そちらを参照してください。

  - PXmonja パッケージ
    <http://zrbabbler.sp.land.to/pxmonja.html>

更新履歴
--------

  * Version 0.2a [2016/02/14]
      - バグ修正。
  * Version 0.2  [2010/06/06]
      - 最初の公開版。

--------------------
Takayuki YATO (aka. "ZR")  
http://zrbabbler.sp.land.to/
