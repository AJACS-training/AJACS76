# AJACS徳島 ゲノムブラウザ／発現・局在関連データベース

大学共同利用機関法人 情報・システム研究機構  
データサイエンス共同利用基盤施設  
ライフサイエンス統合データベースセンター    
[小野 浩雅](https://sites.google.com/a/dbcls.rois.ac.jp/hono/)  
hono@dbcls.rois.ac.jp  
2019年6月6日(木)
AJACS徳島 @ 大塚製薬株式会社 徳島研究所 2研ホール

----

これは統合データベース講習会 AJACS徳島「ゲノムブラウザ／発現・局在関連データベース」の講習資料です。  
講習会全体のプログラムは[こちら](https://biosciencedbc.jp/event/ajacs/ajacs76.html)です。
© 2019 小野 浩雅, [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/deed.ja)

----

## 概要

本講習は、だれでも自由に使うことができる公共データベースやウェブツールを活用して、研究のさまざまな場面で調べることの多い「遺伝子」を中心とした種々の情報を取得する方法について解説します。また、遺伝子発現データという観点で、個々の遺伝子発現データを簡単に調べるための方法と基礎知識について解説します。 さらに、自ら行なった大規模発現解析の(あるいは公共データベースから取得・解析した)結果として得られた数百〜数千におよぶ遺伝子セットについて、生物学的な解釈をする方法とその結果の考察を実践します。  

----

## 講習の流れ
今回の講習では、コンピュータを使って以下の内容について説明します。

- ゲノムデータベース・ゲノムブラウザ
  - UCSC Genome Browser
    - 【実習】UCSC ゲノムブラウザを使ってGTExのデータを閲覧してみる

- 個々の遺伝子の発現プロファイルを調べる
  - RefEx
    - 【実習】RefExを使って、組織特異的遺伝子を検索する

- 数十～数千の遺伝子群の生物学的解釈
  - ChIP-Atlas
    - 【実習】ChIP-AtlasのEnrichment Analysis を使って、興味ある遺伝子リストを制御する可能性の高い転写因子を調べる

- 研究現場で頻繁に使われるデータベースやツールを知る
  - 統合TV

----

## 講義に際しての注意とお願い
- みんなで同時にアクセスするとサイトにつながりにくくなることが予想されます。
    - 資料を見ながら自力で進められそうな方はどんどん先に、そうでない方は講師と一緒にすすめていきましょう。
    - サイトの反応が悪い時はタイミングをずらして実行してみてください。
    - 反応が無いからと言って何度もクリックするとますます繋がらなくなってしまいます。おおらかな気持ちで臨みましょう。
- 実験的な試みとしてWeb上で質問・コメントできるフォームを用意してみました。
    - https://www.sli.do (「新しいタブで開く」とよいです)
     - ウェブブラウザで sli.do と入力(スマホでもアクセス可能)
     - AJ76 と入力
     - 質問をする (ﾟдﾟ)ｶﾝﾀﾝｰ

 - こんなことは知ってて当たり前だと他の人に思われる質問を歓迎します。質問することのハードルを下げます。
    - 知っている人は講師を助けてください。サポート大歓迎です。
    - あなたが疑問に思ったことは、実は、隣の人やその隣の人もそう思っていることが多いです。
    - 当たり前に感じる質問や一見関係なさそうな質問がでると、「そういう質問をしてもよいのだ」という空気になり、この講義から得られる情報が増え、皆さんの受講満足度が上がります(たぶん)。
    - でも講師も知らないことは(多々)あります。(以下ループ)


----

#### 受講前アンケートにご協力いただき、ありがとうございます (回答数 48)(5/28暫定)

|統合TVを知っていますか?|人数|割合|
|:--|--:|:--:|
|知らない|19 名|40 %|
|知っている|23 名|47 %|
|回答なし|6 名|13 %|
---
|自分で実験して得た、数十〜数千の遺伝子からなる<br>「遺伝子リスト」(例: 発現差のあった遺伝子など) を持っていますか?|人数|割合|
|:--|--:|:--:|
|これから実験をする・したい|12 名|25 %|
|公共データを活用する・したい|11 名|23 %|
|既に持っている|11 名|23 %|
|大規模発現解析の予定はない|11 名|23 %|
|回答なし|3 名|6 %|
---

## ゲノムデータベース・ゲノムブラウザ
### ゲノムデータベースとは？
- ゲノム配列をはじめとした（遺伝）情報を生物種ごとにまとめたデータベース
- 狭義にはゲノム配列のデータベースを指す

#### さまざまなゲノムデータベース
- [NCBI](https://www.ncbi.nlm.nih.gov/) (National Center for Biotechnology Information) の [**Genome**](https://www.ncbi.nlm.nih.gov/genome/)
  - [生物種ごと(Browse by Organism)](https://www.ncbi.nlm.nih.gov/genome/browse#!/overview/)
- [GOLD: Genomes Online Database](https://gold.jgi.doe.gov/index)
	- ゲノム塩基配列解読プロジェクトを集めたデータベース
- [PlantGDB](http://www.plantgdb.org)
  - [Plant Genome Database Japan(PGDB)](http://pgdbj.jp/)
- [MicrobeDB.jp](http://microbedb.jp/MDB/)

#### コミュニティによるゲノムデータベース

- Mouse Genome Informatics (MGI) - マウス
	- http://www.informatics.jax.org/
- Rat Genome Database (RGD) - ラット
	- https://rgd.mcw.edu/
- WormBase - 線虫
	- https://www.wormbase.org/
- FlyBase - ショウジョウバエ
	- http://flybase.org/
- The Arabidopsis Information Resource (TAIR) - シロイヌナズナ
	- https://www.arabidopsis.org/
- Saccharomyces Genome Database (SGD) - 酵母
	- https://www.yeastgenome.org/
- CyanoBase - シアノバクテリア（光合成細菌）
	- http://genome.microbedb.jp/cyanobase/

---

### ゲノムブラウザとは？

- 塩基配列解読したゲノム配列とそこに付与（アノテーション）された情報を見るための仕組み
- オンライン型とローカル型
  - オンライン型：ウェブブラウザ上でサーバにあるゲノムデータベースから必要な情報を取り出してこれる
  	- UCSC Genome Browser https://genome.ucsc.edu/
      - 【統合TV】[「UCSC」](https://togotv.dbcls.jp/tags.html?tag=UCSC)のタグ(講習含む計27本の動画)
  	- Ensembl Genome Browser https://www.ensembl.org/
      - 【統合TV】[「Ensembl」](https://togotv.dbcls.jp/tags.html?tag=Ensembl)のタグ(講習含む計25本の動画)
  	- NCBI Genome Data Viewer https://www.ncbi.nlm.nih.gov/genome/gdv/
  	- Togogenome http://togogenome.org/
      - 【統合TV】[TogoGenome を使って生物種とゲノムに関する多種多様な情報を統合的に検索する](https://togotv.dbcls.jp/20180726.html)
  - ローカル型：手元のコンピュータにインストールして使用
  	- Integrative Genomics Viewer(IGV) https://software.broadinstitute.org/software/igv/
      - 【統合TV】[Integrative Genomics Viewer IGVを使い倒す 〜基本編〜](https://togotv.dbcls.jp/20140529.html)

#### 【実習】UCSC ゲノムブラウザを使ってGTExのデータを閲覧してみる

- 【統合TV】: [UCSC Genome Browser を使って様々な組織、細胞における遺伝子発現データをゲノムブラウザで表示する](https://togotv.dbcls.jp/ja/20171116.html)
- 【統合TV】: [GTEx Portalを使ってヒトの各組織での遺伝子発現量や影響するeQTLを調べる](https://togotv.dbcls.jp/20180101.html)
  - [Genotype-Tissue Expression (GTEx)](https://www.gtexportal.org/home/) プロジェクトは米国ブロード研究所(Broad Institute)をはじめとする南北米および欧州の複数の研究機関からなる国際コンソーシアムによる、ヒトの体組織ごと、遺伝子型ごとの遺伝子発現を網羅的に調べたプロジェクトです。 そのポータルサイトであるGTEx Portalでは、GTExプロジェクトで収集・解析された遺伝子の発現量や関連するeQTL(expression Quantitative Trait Locus: 遺伝子の発現量に影響を与える座位)などのデータがまとめられています。


1. 「[UCSC Genome Browser](https://genome.ucsc.edu/)」で、トップページを開きます
1. トップページにはツール名がリストされているので一番上にある「Genome Browser」をクリックします
![UCSCトップページ](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_04.png)
1. 最寄りのミラーサイトに接続します
![UCSC mirror](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_05.png)
1. Genome Browserのページが開くので、生物種「Human」と最新のゲノムアセンブリ「Dec. 2013 (GRCh38/hg38)」が選択されていることを確認して、そのまま「Go」をクリックします
![GenomeBrowserトップページ](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_06.png)
1. Current position: chr1:11,102,837-11,267,747 の領域が表示されます。GTExのトラックは初期設定だと画面中央(赤枠)にあります
![chr1:11,102,837-11,267,747](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_07.png)
1. GTEx のトラックでは組織ごとの遺伝子発現量がバーチャートで表示されており、マウスオーバーすると発現値と組織名が示されます
  - バーチャートの横幅は遺伝子の領域とは無関係であることに注意
  - 横線の色は遺伝子のタイプを示し、青はprotein-coding、緑はnon-coding、ピンクはpseudogene
![マウスオーバー](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_08.png)
1. グラフ自体をクリックすると詳細情報を閲覧できます
  - トラック上のバーチャートでは発現値はlog10変換されているが、詳細情報の箱ひげ図ではlog10変換されていないことに注意
![箱ひげ図](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_09.png)
1. 一つ前のページに戻って、下部に移動すると「GTEx Gene」のトラックがあるので、そこをクリックすると設定画面に移動します
![GTEx Geneトラック](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_10.png)
 - デフォルトでは、全ての組織が表示されるようになっています。特に比較したい組織がある場合は、Clear allをクリックして選択を解除してから、目的の組織だけを選択します
 - 発現値のlog10変換はこの画面で設定変更できます
1. 一つ前のページに戻って、「track hubs」を活用すると、GTExデータのようなUCSC外部のデータソースに由来する様々なアノテーショントラックを追加できます。
![track hubs](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_11.png)
1. 細胞ごとのmiRNAの発現量を表示できるトラック「Human cellular microRNAome barChart」を選択して「Connect」をクリックします
 - 3つの異なる研究データに基づくヒトの78の初代培養細胞と42のがん細胞あるいは不死化細胞のmiRNA発現量を測定したデータです([原著論文: Toward the human cellular microRNAome](https://genome.cshlp.org/content/27/10/1769))
![Human cellular microRNAome barChart](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_12.png)
1. 自動的に画面が遷移してGenome Browserのトップページに戻るので、検索したいmiRNA(今回は例としてMIR126)を検索窓に入力します。
![search for MIR126](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_13.png)
1. [MIR126の領域](https://genome.ucsc.edu/cgi-bin/hgTracks?db=hg38&lastVirtModeType=default&lastVirtModeExtraState=&virtModeType=default&virtMode=0&nonVirtPosition=&position=chr9%3A136670602%2D136670686&hgsid=727916439_U4isI9rJMtlZRcqlhIG7YGeB53Lv)のデータがバーチャートで表示されます。
![MIR126](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_14.png)
1. その他、いろいろ変更して表示してみましょう。わからなくなったら、図の下に並んでいるボタンの「default tracks」を押すと最初の状態に戻せます。

- 設定変更や追加で表示可能なアノテーションを調べる方法
  - 【統合TV】: [UCSC Genome Browserで表示できるアノテーションを調べる 2018](https://togotv.dbcls.jp/20180710.html)

---


## 個々の遺伝子の発現プロファイルを調べる

### 誰でも使える公共の遺伝子発現データ
- さまざまな実験で得られたデータは、論文投稿時などに公共データベース上に登録し、その後誰でも参照可能になるようにすることが義務付けられていることが多いですが、それは遺伝子発現データについても同様です。公共データベースには多種多様な遺伝子発現データが日々大量に登録、蓄積され続けています。
  - これらのデータをうまく活用すれば、例えば、予備実験をせずに済む、自分の実験結果を支持する知見が得られる、仮説立案の新たな切り口が得られるなど、多くのメリットがあります。
  - 一方で、いざ使おうと思ったときに、その膨大さから、どのデータを選び、詳しく調べればよいのか分かりにくく、利用することが困難で諦めてしまうことが多いです。
- これらの困難さを軽減するために、いくつかの二次的なデータベースやツールが開発されています。これらをうまく使うことで、自分のデータと組み合わせられる遺伝子発現データをすばやく検索、発見し、活用できるようになるでしょう。

### [RefEx (Reference Expression dataset)](https://refex.dbcls.jp/)
- 遺伝子発現解析の基準となるデータを快適に検索できるウェブツール
    - [https://refex.dbcls.jp/](https://refex.dbcls.jp/)
    ![Fig-1](https://raw.githubusercontent.com/dbcls/website/master/services/images/DBCLSservices_RefEx_jp_fig-1_180523.png)  

    ![Fig-2](https://raw.githubusercontent.com/dbcls/website/master/services/images/DBCLSservices_RefEx_jp_fig-2_180523.png)
    ![fig-3'](https://raw.githubusercontent.com/dbcls/website/master/services/images/DBCLSservices_RefEx_jp_fig-3_180523.png)
- 公共DBにある正常組織や細胞株における遺伝子発現データを再利用・整理
- 4つの異なる実験手法（EST、GeneChip、CAGE、RNA-seq）によって得られた正常組織、初代培養細胞、細胞株における遺伝子発現データを検索、閲覧可能
    - FANTOM5 CAGEデータ(phase1)も閲覧可能です(ヒト556種、マウス286種)
      - FANTOM5 CAGEデータ
        - 理化学研究所のFANTOM プロジェクト5（[FANTOM5](http://fantom.gsc.riken.jp/5/)）では、ゲノムにコードされているプロモーターと転写因子制御ネットワークを明らかにすることを目的として膨大なCAGEデータを測定し、それらを閲覧できるウェブサイトも公開されている。
    - 掲載しているデータやオリジナルデータなどの詳細については、[RefExについて](https://refex.dbcls.jp/about.php?lang=ja)
- このツールでできること
    - 正常組織における遺伝子発現データを調べる
    - 測定手法による遺伝子発現量の差異を比較する
    - 組織特異的遺伝子をワンタッチで検索可能
    - 遺伝子発現解析などで見出された不詳な遺伝子群の機能および関係性を調べる
- RefExで掲載されているデータはすべて再利用可能
    - オリジナルデータの再処理方法の詳細は[GitHub](https://github.com/dbcls/RefEx/tree/master/Rawdata_Processing)に
    - 再処理済みの発現データやサンプルアノテーション等のすべてのデータは[figshare](https://figshare.com/)に
    - 「The RefEx analysis」として論文に引用していただいた活用例
    	- [Aberrant IDH3α expression promotes malignant tumor growth by inducing HIF-1-mediated metabolic reprogramming and angiogenesis, Oncogene, (22 December 2014) | doi:10.1038/onc.2014.411 @ Figure 6](http://www.nature.com/onc/journal/vaop/ncurrent/full/onc2014411a.html)
        - がん研究者が、発現解析実験で見出した数百個の治療標的・候補遺伝子の絞込みに使えないか検討した。
        - これらの候補遺伝子の正常組織における発現量が低ければ、治療標的とした場合に悪影響・副作用が小さくなると仮説した。
        - 実際に、これらの遺伝子の発現量をRefExで確認し、追加確認実験の優先順位付けを効率的に行うことができた。
    - その他RefExを引用した論文の一覧はこちらでご覧いただけます。
        - [https://dbcls.rois.ac.jp/references.html#RefEx](https://dbcls.rois.ac.jp/references.html#RefEx)

#### 参考文献
  * Hiromasa Ono, Osamu Ogasawara, Kosaku Okubo, Hidemasa Bono
     **RefEx, a reference gene expression dataset as a web tool for the functional analysis of genes**
             Scientific Data, 4:170105
             [DOI: 10.1038/sdata.2017.105](http://doi.org/10.1038/sdata.2017.105)
  * 川路 英哉、粕川 雄也、坊農 秀雅、小野 浩雅 「FANTOM5データを誰でも活用できる形に」 Scientific Data誌著者インタビュー (平成29年8月29日)
             https://www.natureasia.com/ja-jp/scientificdata/papers-from-japan/fantom5
  * 小野 浩雅・坊農 秀雅 「遺伝子発現解析の基準となるデータを快適に検索できるウェブツールRefEx」 ライフサイエンス新着論文レビュー (平成29年9月5日)
             [DOI: 10.7875/first.author.2017.093](http://doi.org/10.7875/first.author.2017.093)
  * 統合TV 「RefExの使い方」[DOI: 10.7875/togotv.2014.009](http://doi.org/10.7875/togotv.2014.009)
----

#### 【実習】RefExを使って、組織特異的遺伝子を検索する
- 【統合TV】[RefExの使い方](https://doi.org/10.7875/togotv.2014.009)

1. https://refex.dbcls.jp/ を開きます。
2. 画面中央の「組織特異的に発現する遺伝子を見る」の臓器アイコンにカーソルを合わせると、更に詳細な部位のアイコンが出るので、調べたい臓器（例として肝臓）をクリックします。  
  - ![http://gyazo.com/35c8f38340753e8f433cb8c4d8fd812b](http://i.gyazo.com/35c8f38340753e8f433cb8c4d8fd812b.jpg)

3. 検索結果一覧が表示されます。検索結果一覧では、「ソート項目の切り替え」や「絞り込み検索」、「リストへの追加」ができます。(手順11以降で解説します。)
4. 各遺伝子の青字の部分（例 [fibrinogen alpha chain](https://refex.dbcls.jp/gene_info.php?lang=ja&db=human&geneID=2243&refseq=NM_000508&unigene=Hs.351593&probe=205649_s_at))をクリックすると詳細情報を閲覧できます。
5. 「ヒートマップ on Bodyparts3D」では、表示する部位の切り替え（全身・体幹部・頭部）ができます。「皮膚・骨格筋を表示」もしくは「アニメーション表示」にチェックを入れるとどのように表示されるでしょうか。
6. 「組織40分類別データ」では、バーの上にマウスオーバーすると測定部位と発現値が表示されます。
7. 「Download」をクリックすると、表示中の遺伝子の組織40分類別の発現データがタブ区切り形式でダウンロードできます。
8. 「Probe set ID」のリンク先をクリックすると、どういう情報が参照できるでしょうか。
9. 遺伝子オントロジー([Gene Ontology](http://array.cell-innovator.com/?p=1085):GO ID)をクリックすると、そのGO termを持つ他の遺伝子を一括で検索できます。
  - 例として、[GO:0007596](https://refex.dbcls.jp/genelist.php?lang=ja&db=human&idkind=1&ids=GO:0007596)   blood coagulation をクリックしてみましょう。
  - ![遺伝子詳細情報](http://i.gyazo.com/3cca3d33c17e845ad5dae8749d7fbd15.jpg)

10. 右側のFANTOM5 CAGEのタブをクリックすると、FANTOM5 CAGEデータのビューアに切り替わります。
 - ビューアは上部が拡大図で、下部が全体表示になっています。
 - 検索窓にキーワードを入れるとサンプル名を検索できます。ヒットしたサンプルはオレンジ色で強調されます。
 - 右側に、サンプル名と発現値、サンプル分類が表示されます。
 - [RefEx用に整理したサンプル情報一覧](http://bit.ly/fantom5cagehuman)も閲覧可能です。
 - ![FANTOM5 CAGE Viewer](http://i.gyazo.com/51d0b3db07efe64a6fdafb054cd4217f.jpg)
11. 検索結果一覧に戻ります。ソート項目を切り替えて、どのように結果が変わるでしょうか。
 - ![検索結果一覧](http://i.gyazo.com/5e87d20d9b31711e797ef17677be7263.jpg)
12. 様々な条件で検索結果を絞り込むことができます。絞り込み検索は左のバーから行えます。
 - 遺伝子名に「liver」を含むデータは何件あるでしょうか。
 - 「遺伝子名」の下の「条件なし」をクリックして表示されるウインドウに「liver」と入力し、「Include」をクリックし、「この条件で絞り込み」を押します。
 - 「遺伝子名」の項目で「Exclude」に「solute」を加えると、検索結果はどう変わるでしょうか。
 - 「組織」の項目で、データ元をRNA-seqに変更したり、臓器の指定を追加すると検索結果はどう変わるでしょうか。
 - 「必ず含むデータセット」の「ALL」にチェックを入れると、検索結果はどう変わるでしょうか。
13.  個々の遺伝子の詳細情報は、リストに追加することで並列に比較することができます。
 - [肝臓特異的遺伝子の検索結果一覧](https://refex.dbcls.jp/genelist.php?lang=ja&db=human&roku_valid=1&rk[31]=31&order_key=score)に移動して、3つの遺伝子を「リストに追加」してみましょう。
 - 追加した件数は「リストを見る」の横に表示されます。
 - 「リストを見る」をクリックするとリストに移動します。
 - 『並べて表示する』にチェックを入れて、「遺伝子を並べて表示」をクリックします。
 - 遺伝子発現データやGeneOntology情報を並列に比較することで見えてくる「違い」はなんでしょうか。その違いからどういうことが推測できるでしょうか。
 - ![並列比較1](http://i.gyazo.com/ba11e4c7c38a4e78d3a64d7b8b6efee8.jpg)
 - ![並列比較2](http://i.gyazo.com/3f2f9e5cbf135a2c298ae164d6360302.jpg)
14. 自分の研究テーマに関連する、また興味のある遺伝子について検索してみましょう。

#### 関連するツール
- ExpressionAtlas
  - Expression Atlas は、EMBL-EBI (欧州バイオインフォマティクス研究所) が運営する、様々な生物種における遺伝子発現情報を提供するウェブサイトである。40 の生物種について、3000 以上の実験に基づき、組織や細胞種、発生段階、疾患の有無などの条件別に、遺伝子の発現情報をまとめられています。
  - 【統合TV】[Expression Atlas で 様々な生物種の組織や疾患などにおける遺伝子発現の情報を調べる](https://togotv.dbcls.jp/20180725.html)

- Bgee
  - Bgee (a dataBase for Gene Expression Evolution: ビージーと発音します) は、SIB Swiss Institute of Bioinformatics/ローザンヌ大学の Robinson-Rechavi Group - Evolutionary Bioinformaticsが提供するデータベースで、これはRNA-seqやマイクロアレイなどから得られた遺伝子発現パターンについて、多くの生物種間で比較することができます。
  - 【統合TV】[Bgee を使って、複数の生物種の正常組織における遺伝子発現データを検索、比較、取得する](https://togotv.dbcls.jp/20180918.html)

- BioGPS
  - AffymetrixのマイクロアレイであるGeneChipを用いたヒト、マウス、ラットを始め全9生物種におけるさまざまな組織や細胞(株)における遺伝子発現プロファイルのデータベースです。
  - 【統合TV】[遺伝子発現プロファイルデータベースBioGPSを使い倒す 2012](https://togotv.dbcls.jp/20120911.html)

----

## 数十～数千の遺伝子群の生物学的解釈

- マイクロアレイやNGS実験を行うと大量の発現変動遺伝子 (Differentially Expressed Genes: DEGs)が得られます｡
- 一般的な遺伝子発現解析の第一歩は､実験条件によって得られた数十～数千のDEGsが生物学的にどういう意味を持つかを考えることです。
  - ![Gyazo](http://i.gyazo.com/52cb4c40b1313a52f8ded6923bdd8ef0.png)

### ChIP-Atlas
ChIP-Atlasは、論文などで報告された ChIP-seq データを閲覧し、利活用するためのウェブサービスです。データ処理の知識やスキルがない方でも簡単に利用できます。データソースは、公開 NGS データレポジトリ (NCBI, EMBL-EBI, DDBJ) に登録されたほぼ全ての ChIP-seq データです。ChIP-Atlas は、九州大学大学院医学研究院 発生再生学分野 (http://www.dev.med.kyushu-u.ac.jp) と DBCLS が共同で開発しています。  
 (https://chip-atlas.org/)

![fig10](https://raw.githubusercontent.com/hiromasaono/training/master/images/181104_10.png)

![fig11](https://raw.githubusercontent.com/hiromasaono/training/master/images/180612_11.png)

#### ChIP-Atlasの機能
##### Peak Browser
- 既報の ChIP-seq データをまとめて閲覧し、何がどこに結合しているかが一目でわかります。Integrative Genomics Viewer (IGV) によりスムーズなブラウジングが可能で、興味の遺伝子のシス調節領域を予測したり、それを制御する転写因子の予測ができます。
  - 【統合TV】[ChIP\-Atlasを使って既報のChIP\-seqデータをまとめて閲覧する 〜Peak Browserの使い方〜](https://togotv.dbcls.jp/20180123.html)
##### Target Genes
- 興味のある転写因子を選択し、その標的遺伝子候補を検索できます。
  - 【統合TV】「[ChIP\-Atlasを使って興味のある転写因子を選択しその標的遺伝子候補を検索する 〜Target Genesの使い方〜](https://togotv.dbcls.jp/20180124.html)」
##### Colocalization
- 興味のある転写因子を選択し、それとゲノム上で共局在する転写因子候補を検索できます。
  - 【統合TV】「[ChIP\-Atlasを使って共局在タンパク質を探す 〜Colocalizationの使い方〜](https://togotv.dbcls.jp/20180128.html)」
##### Enrichment Analysis
  - ユーザデータを受け付け、既存データとの比較解析をおこないます。たとえば、興味のある遺伝子リストを submit すると、それらをまとめて制御する転写因子候補が返されます。ほかにも BED 形式のファイルや、シーケンスモチーフを submit すると、それらに enrichment する転写因子群が返されます。


#### 利用例
- 論文として発表された ChIP-Seq データを閲覧したい
- 興味のあるゲノム領域における、転写因子や修飾ヒストンの分布を知りたい
- 興味のある転写因子の下流遺伝子や、複合体形成パートナーを知りたい
- 自身の研究データと公開 ChIP-seq データを用いて比較解析をおこないたい

#### 参考文献
- Source code and documentation    
  - https://github.com/inutano/chip-atlas
- Preprint
  - Shinya Oki, Tazro Ohta, et al. Integrative analysis of transcription factor occupancy at enhancers and disease risk loci in noncoding genomic regions. bioRxiv 262899; doi: https://doi.org/10.1101/262899
- Paper
  - Shinya Oki, Tazro Ohta, Go Shioi, Hideki Hatanaka, Osamu Ogasawara, Yoshihiro Okuda, Hideya Kawaji, Ryo Nakaki, Jun Sese, and Chikara Meno.
     **ChIP-Atlas: a data-mining suite powered by full integration of public ChIP-seq data.**
              EMBO Reports
             [https://doi.org/10.15252/embr.201846255]( https://doi.org/10.15252/embr.201846255)  
- Database
  - Oki, S; Ohta, T (2015): ChIP-Atlas. http://dx.doi.org/10.18908/lsdba.nbdc01558-000
- Publications citing ChIP-Atlas http://chip-atlas.org/publications

### 【実習】ChIP-AtlasのEnrichment Analysis を使って、興味ある遺伝子リストを制御する可能性の高い転写因子を調べる
- 「発現差のあった遺伝子リスト」を持っている想定で、それらの遺伝子に結合しうる、あるいは上流でそれらの遺伝子の発現を制御する可能性がある転写因子を検索する
- 使用するデータ
  - [190606_List_of_GeneSymbol_txt](https://github.com/AJACS-training/AJACS76/blob/master/05_hono/190606_List_of_GeneSymbol.txt)
    - ある「興味ある遺伝子リスト」をGeneSymbolにID変換したデータ。
    - これを使って、もともとどういう遺伝子リストだったかを考察します。
  - ChIP-Atlas では、遺伝子IDとしてGeneSymbolのみを受け付けているので、それ以外のIDで遺伝子リストを持っている場合は、適宜変換が必要です。
    - ID変換はいろいろなツールがありますが、今回は[HGNC BioMart](https://biomart.genenames.org/)を利用します。
      - HGNC(The HUGO Gene Nomenclature Committee)はヒトのGeneSymbolを認定・管理している機関。
        - 【統合TV】[HGNCを使ってヒト遺伝子の正式略称(GeneSymbol)を検索する(+ヒトとマウスの遺伝子IDを変換する)](https://togotv.dbcls.jp/20190406.html)
      - [DAVID(Database for Annotation, Visualization and Integrated Discovery)
   ](https://david.ncifcrf.gov/)のGene ID Conversion Toolも便利。([使い方動画](https://youtu.be/4f1t1ma9IRc?t=4m5s))


1. [ChIP\-Atlas - Enrichment Analysis](https://chip-atlas.org/enrichment_analysis)にアクセスします。
1. 下図のようにオプションを設定します。
![fig12](https://raw.githubusercontent.com/hiromasaono/training/master/images/181104_12.png)
1. submit すると遺伝研スパコンへクエリが飛びます。(ので、講義中は見てるだけにしてください)
1. submit したあとの画面
![fig13](https://raw.githubusercontent.com/hiromasaono/training/master/images/181104_13.png)
1. 計算が終わるまで待ちます
![fig14](https://raw.githubusercontent.com/hiromasaono/training/master/images/181104_14.png)
1. 計算が終わると、「Result URL」が有効になります。
  - 今回の例では、 http://ddbj.nig.ac.jp/wabi/chipatlas/wabi_chipatlas_2018-1104-1735-21-275-473936?info=result&format=html
1. 結果の解釈をします。
  - 今回は、どういう「興味ある遺伝子リスト」をクエリとしたか考察してみましょう。
  - 「p-valueが低く、Overlaps/My dataが多く、Fold Enrichmentが高い」転写因子がたくさんヒットしてくる　
    - → 入力した遺伝子群をまとめて制御する、マスター転写因子を抽出できている可能性が高いと言えます。

1. [答え合わせ](https://github.com/AJACS-training/AJACS76/blob/master/05_hono/190606_ChIP-Atlas_answer.md)



## 研究現場で頻繁に使われるデータベースやツールを知る
### [統合TV](https://togotv.dbcls.jp/)
#### 生命科学分野の有用なデータベースやツールの使い方を動画で紹介するウェブサイト
- https://togotv.dbcls.jp/
- ![統合TVトップページ](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_01.png)
- 各動画は[YouTubeに上がって](http://www.youtube.com/user/togotv/)おり、おなじみの再生画面で快適にご覧いただけます。(環境に応じた解像度、倍速表示等)
- 1600本を超える動画が公開されており、YouTube版だけで のべ 1,300,000回以上 再生されています。(2019年4月末現在)
- ![YouTube統計](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_03.png)
- ![統合TV 再生画面](https://raw.githubusercontent.com/hiromasaono/training/master/images/190606_02.png)
  - ウェブサイトへのアクセスの仕方から結果の解釈まで、操作の一挙手一投足がわかります。
  - 動画ファイルのみの一部および一括ダウンロード([NBDC生命科学系データベースアーカイブ](https://dbarchive.biosciencedbc.jp/jp/togotv/download.html))も可能で、オフライン視聴もできます。
  - 動画の概要を示すダイジェスト見出しで視聴すべき箇所がわかりやすくなっています。
  - 各動画には、恒久的な URL として利用されている [DOI](https://ja.wikipedia.org/wiki/デジタルオブジェクト識別子) (Digital Object Identifier) が付与されています(引用可能)。
  - 講義・講習などの参考資料や後輩指導の教材として利用できます。
    - 本講義中も、本家サイトが繋がらない時は、統合TVを見ればおおよその内容がわかるようになっています。

#### 動画以外のコンテンツも拡充中
- [AJACS講習会資料](https://togotv.dbcls.jp/ja/ajacs_text.html)
  - 2014年8月以降に開催された過去の講習会の資料・テキストと動画が同時閲覧できます。
  - 受講生の復習のみならず、初学者の学習教材として活用できます。
- [Togo Picture Gallery(静止画)](https://togotv.dbcls.jp/ja/pics.html)
  - 誰でも自由に利用可能なライフサイエンス分野のイラストが､統合TVから閲覧､利用することができるようになりました。[「自由に使える画像を探す」](https://togotv.dbcls.jp/ja/pics.html)
  - Togo picture galleryと[生物アイコン](https://togodb.biosciencedbc.jp/togodb/view/taxonomy_icon)の全画像500点以上を一覧できます。
  - 研究発表のスライド作成や資料作成等に､ぜひお使いください。
  - ![自由に使える画像を探す](https://raw.githubusercontent.com/hiromasaono/training/master/images/180612_04.png)

#### 募集と宣伝
- お探しの動画・静止画が見つからない場合は、[統合TV番組リクエストフォーム](https://togotv.dbcls.jp/ja/contact.html)でお気軽にリクエストを。
- 統合TVでコンテンツを作ってみたい方も募集中です。
  - オンラインで完結する作成環境を整備しており、遠隔地でもOKです。謝金あり。)
- 統合TVを効果的に利用するためのガイドブックが出版されました。(2018年12月)
  - 生命科学データベース・ウェブツール  － 図解と動画で使い方がわかる！ 研究がはかどる定番18選 －
  - 「定番」として何がよく使われているのかを知り、その使い方を学び、どう使うと便利なのかについて、体系的にまとめて俯瞰的に捉えられるように編集されています。
  - 「この順で動画をみていくと、こういうスキルを獲得できる」というような体系的な教材です。
  - https://www.amazon.co.jp/dp/4815701431/
  - https://www.medsi.co.jp/books/products/detail.php?product_id=3665

    ----

#### 習熟度ややりたいこと別に、とりあえず押さえておきたい統合TVオススメ番組
- DBCLSの提供する便利な各種サービスをレビュー
  - [【NGSハンズオン2017】NBDC・DBCLSの各種サービス 今日から使える便利な生命科学系公共データベース in DBCLS](https://togotv.dbcls.jp/20171204.html)

- PubMed検索のプロによる文献検索のイロハを学ぶ
  - [文献情報を用いたサービスを活用する @ AJACS越後](https://togotv.dbcls.jp/ja/ajacs2018011.html)

- 塩基配列解析に関わる基礎知識(遺伝子IDとそのデータベース)とゲノム編集について
  - [塩基配列解析およびゲノム編集のためのデータベース・ウェブツール](https://togotv.dbcls.jp/ja/ajacs2018021.html)

- 次世代シーケンス(NGS)データ解析に必要な基礎知識とリテラシーを学ぶ
  - [NGSデータから新たな知識を導出するためのデータ解析リテラシー @ AJACS浜松](https://togotv.dbcls.jp/ja/ajacs2018008.html)

- NGS解析について、さらにもっと基礎から応用までを深く学びたい方向け (それぞれ約50時間程度)
  - [「バイオインフォマティクス人材育成カリキュラム（次世代シークエンサ）速習コース(2014年8月)](https://www.youtube.com/playlist?list=PL0uaKHgcG00abmj1Nzs1SUhqKLjf_PFBB)
  - [「バイオインフォマティクス人材育成カリキュラム 次世代シークエンサ(NGS)ハンズオン講習会(2015年8月)](https://www.youtube.com/playlist?list=PL0uaKHgcG00Yo0Cn0rcF23xof5hqCzGQb)
  - [NGSハンズオン講習会2016](https://www.youtube.com/watch?v=TSa1yPy_sdM&list=PL0uaKHgcG00ZNpICun17CEAFpV_5Q6GCA)
  - [NGSハンズオン講習会2017](https://www.youtube.com/watch?v=6Fzvl_I48tM&list=PL0uaKHgcG00YDmBXYWOgkmfeURjc8BZkk)
  - [上記の動画+講習会資料のまとめページ@統合TV](https://togotv.dbcls.jp/ja/tags.html?tag=NGS速習・ハンズオン)

- データ可視化・解析ツール
  - [Tableau Public を使って 行列データを直感的に可視化し解析する](https://togotv.dbcls.jp/20181126.html)
  - [Morpheus を使って、様々な行列データをヒートマップで表示しウェブブラウザでデータ解析をする](https://togotv.dbcls.jp/20181109.html)
  - [Dataset2Tools でオミックスデータとその解析事例、計算ツールを検索し、再現性の高い再解析を行う](https://togotv.dbcls.jp/20181021.html)
      - [Enrichr](http://amp.pharm.mssm.edu/Enrichr)


- ビッグデータ時代の疾患ゲノム解析で使いこなしたいデータベース
  - [The Cancer Genome Atlas \(TCGA\) を使って各癌種の公開データを検索・ダウンロードする](https://togotv.dbcls.jp/20171210.html)
  - [The Cancer Genome Atlas \(TCGA\) を使って各癌種の公開データを解析する](https://togotv.dbcls.jp/20171214.html)
  - [COSMICでがん遺伝子の体細胞変異について調べる](https://togotv.dbcls.jp/20180127.html)
  - [COSMIC\-3Dを使って がん遺伝子のコードするタンパク質の立体構造を がんで見られる変異の情報と重ねて見る](https://togotv.dbcls.jp/20180329.html)
  - [depmapを使ってがん細胞が依存する遺伝子の情報を調べる \(がんの治療標的となる遺伝子を発見する\)](https://togotv.dbcls.jp/20180531.html)
  - [GWAS Catalog を使って、GWASで見つかった形質と多型の関連について検索する](https://togotv.dbcls.jp/20180402.html)
  - [ClinVarで疾患に関連する変異を検索し、Variation Viewerで視覚的に変異を探す](https://togotv.dbcls.jp/20180122.html)
  - [gnomADを使ってヒトのエキソームやゲノムのデータから変異を探す](https://togotv.dbcls.jp/20180401.html)
    - [GTEx Portalを使ってヒトの各組織での遺伝子発現量や影響するeQTLを調べる](https://togotv.dbcls.jp/20180101.html)
    - [TogoVar でヒトゲノムに存在するバリアントに関連する情報を調べる](https://togotv.dbcls.jp/20180825.html)

----



## まとめ
- つまみ食い的ではありますが、ゲノムブラウザから始まり遺伝子発現・局在データに関する(ごく一部の)データベース・ウェブツールの使い方を紹介しました。
- データベースやウェブツールは、顕微鏡 や 実験試薬 などと同じ「道具(ツール)」なので使ってナンボです。
- 便利な「道具」を知って、その使い方が分かれば、あとは情報分析力と想像力の勝負です。
  - 正面からしか見られなかったものが横や後ろやナナメから見ることができて初めて気づくことがあるかもしれません。
- 仮説構築から始まり、実験計画・検証、データ解析、そして論文執筆(以下ループ)という研究サイクルを加速化・効率化していきましょう。
- データベースやウェブツールで困ったら、「統合TV」でまず探して・見てみる
- 研究に役立ったら、ぜひ引用・クレジットを!
  - NBDC/DBCLSの提供するサービス(あるいはそれ以外でも)が、あなたの研究に役立ったら、どんなに些細な事でもぜひ引用(論文、URL等)してください。NBDC/DBCLSの活動は、提供するサービスがどのくらい活用されたかについて主に引用数やアクセス数などで評価されており、利用者の方の積極的なサポートが必要不可欠です!!
  - [NBDC関連サービスの活用に関する情報提供フォーム](https://form.jst.go.jp/enquetes/nbdcexamples)


-----
