<meta content="text/html; charset=UTF-8" http-equiv="content-type">

<span class="c32">統合データベース講習会：AJACS徳島</span>

<span class="c31">化合物データベース（Pubchem,ChEMBL）</span>

<span class="c31">&nbsp;〜化合物情報とバイオアッセイ〜</span>

<span class="c24 c35"></span>

* <span class="c41">公益財団法人野口研究所 山田一作（やまだいっさく） </span><span class="c10 c41">[issaku@noguchi.or.jp](mailto:issaku@noguchi.or.jp)</span>

* <span class="c41">日時：2019年6月6日（木）</span>

---

<span class="c3"></span>

<span class="c3"></span>

<span class="c14">1. 目次</span>

<span class="c12 c10">2. 化合物データベース</span>

<span class="c12 c10">3. 参考サイト</span>

<span class="c12 c10">4. PubChem</span>

<span class="c12 c10">PubChemの説明</span>

<span class="c12 c10">PubChem CompoundとSubstanceの違い</span>

<span class="c12 c10">PubChem BioAssayとSubstance</span>

<span class="c12 c10">PubChemへのデータ登録について</span>

<span class="c12 c10">インターフェイスが今年３月に更新。</span>

<span class="c12 c10">ウェブブラウザを用いた検索</span>

<span class="c12 c10">キーワード検索から：遺伝子名：ACADM</span>

<span class="c12 c10">URLへキーワード（遺伝子名、生物種など）を用いた検索</span>

<span class="c12 c10">PubChem Classification Browserを使ったデータ取得</span>

<span class="c12 c10">5. ChEMBL</span>

<span class="c12 c10">ChEMBLの説明</span>

<span class="c12 c10">ウェブブラウザを利用して</span>

<span class="c12 c10">ChEMBLのサイト（https://www.ebi.ac.uk/chembl/）を開く</span>

<span class="c12 c10">概要</span>

<span class="c12 c10">含まれるデータの俯瞰</span>

<span class="c12 c10">階層</span>

<span class="c12 c10">年代毎の分子の種類の分布</span>

<span class="c12 c10">Taxonomyによる分類</span>

<span class="c12 c10">開発フェーズとUSAN登録</span>

<span class="c12 c10">病気のフェーズ</span>

<span class="c12 c10">化合物</span>

<span class="c12 c10">機能の説明</span>

<span class="c12 c10">表示切り替え</span>

<span class="c12 c10">絞り込み</span>

<span class="c12 c10">データダウンロード</span>

<span class="c12 c10">アッセイ</span>

<span class="c12 c10">targets</span>

<span class="c12 c10">キーワード検索</span>

<span class="c12 c10">化合物・医薬品</span>

<span class="c12 c10">遺伝子名</span>

<span class="c12 c10">付録：ドキュメント作成手順</span>

<span class="c3"></span>

---

<span class="c3"></span>

<span class="c3"></span>

<span class="c14">2. 化合物データベース</span>
=====================================

* <span class="c3">AJACS筑波４での化合物データベースについての説明へ</span>

* <span class="c22">[Integbioデータベースカタログ](https://www.google.com/url?q=https://integbio.jp/dbcatalog/?lang%3Dja&sa=D&ust=1559232913839000)</span>

* <span class="c10">[https://github.com/AJACS-training/AJACS70/tree/master/03_yamada](https://www.google.com/url?q=https://github.com/AJACS-training/AJACS70/tree/master/03_yamada%23%25E5%258C%2596%25E5%2590%2588%25E7%2589%25A9%25E3%2583%2587%25E3%2583%25BC%25E3%2582%25BF%25E3%2583%2599%25E3%2583%25BC%25E3%2582%25B9&sa=D&ust=1559232913840000)</span>

<span class="c3"></span>

---

<span class="c3"></span>

<span class="c14">3. 参考サイト</span>
=================================

* <span class="c3">化合物の表記法やPubChemの使い方</span>

* <span class="c3">ブラウザを用いた方法について</span>
* <span class="c3">REST, SOAP, FTPによるデータ取得などについて</span>

* <span class="c10">[https://github.com/yamadaissaku/ChemDocsJP](https://www.google.com/url?q=https://github.com/yamadaissaku/ChemDocsJP&sa=D&ust=1559232913841000)</span>
* <span class="c10">[https://github.com/yamadaissaku/ChemInfo](https://www.google.com/url?q=https://github.com/yamadaissaku/ChemInfo&sa=D&ust=1559232913841000)</span>

* <span class="c3">統合TV</span>

* <span class="c3">PubChemを利用して化学物質やアッセイの結果を調べる 2017</span>

* <span class="c10">[https://togotv.dbcls.jp/20171208.html](https://www.google.com/url?q=https://togotv.dbcls.jp/20171208.html&sa=D&ust=1559232913842000)</span>

<span class="c3"></span>

---

<span class="c3"></span>

<span class="c14">4. PubChem</span>
===================================

<span class="c19">PubChemの説明</span>
-----------------------------------

* <span class="c10">[Web検索](https://www.google.com/url?q=https://www.google.com/search?q%3Dpubchem%26oq%3Dpubchem%26aqs%3Dchrome..69i57j69i60l4j0.4321j0j4%26sourceid%3Dchrome%26ie%3DUTF-8&sa=D&ust=1559232913843000)</span>
* <span class="c3">PubChem公式</span>

* <span class="c10">[pubchemdocs](https://www.google.com/url?q=https://pubchemdocs.ncbi.nlm.nih.gov/&sa=D&ust=1559232913843000)</span>

### <span class="c42">PubChem CompoundとSubstanceの違い</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 316.09px; height: 748.70px;">![](images/image24.png)</span>

### <span class="c42">PubChem BioAssayとSubstance</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 393.33px;">![](images/image100.png)</span>

### <span class="c42">PubChemへのデータ登録について</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 536.00px;">![](images/image98.png)</span>

---

<span class="c3"></span>

<span class="c19">インターフェイスが今年３月に更新。</span>
------------------------------------------

* <span class="c10">[https://pubchemdocs.ncbi.nlm.nih.gov/about](https://www.google.com/url?q=https://pubchemdocs.ncbi.nlm.nih.gov/about&sa=D&ust=1559232913845000)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px -0.00px; border: 1.33px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 529.00px; height: 83.00px;">![](images/image66.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 342.67px;">![](images/image25.png)</span>

---

<span class="c3"></span>

<span class="c19">ウェブブラウザを用いた検索</span>
--------------------------------------

### <span>キーワード検索から：遺伝子名：</span><span class="c32">ACADM</span><span class="c42">&nbsp;</span>

1.  <span class="c10">[中鎖アシル CoA デヒドロゲナーゼ (MCAD) 欠損症の病因遺伝子 ：ACADM ](https://www.google.com/url?q=https://www.genome.jp/dbget-bin/www_bget?ds_ja:H00488&sa=D&ust=1559232913846000)</span><span class="c3">について調べてみましょう。</span>
2.  <span>PubChemのサイト（</span><span class="c10">[https://pubchem.ncbi.nlm.nih.gov/](https://www.google.com/url?q=https://pubchem.ncbi.nlm.nih.gov/&sa=D&ust=1559232913847000)</span><span class="c3">）を開きます。</span>

* <span class="c3">または、Googleなどの検索エンジンで”PubChem”と検索し、下記のリンクをクリック</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 457.81px; height: 98.82px;">![](images/image6.png)</span>

1.  <span>下図のようにキーワード入力欄に”</span><span class="c32">ACADM</span><span class="c3">&nbsp;”を入力すると、Compound, Gene, Taxonomyに分類された候補キーワードが示されます。</span>

<span class="c3"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 402.67px;">![](images/image2.png)</span>

<span class="c3"></span>

1.  <span class="c3">今回は、"Gene"の"Acadm"をクリックすると、下図のサイトに移動します。</span>
2.  <span class="c3">ここでも、分類としてSubstances, Genes, BioAssays, Literature, Patentsが表示され、その下の（）内に含まれるデータの数が表示されます。</span>

<span class="c3"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 401.33px;">![](images/image78.png)</span>

<span class="c3"></span>

1.  <span class="c3">ここで、"Gene"をクリックすると、taxonomy IDの異なる３個の遺伝子が含まれることがわかります。</span>

* <span class="c10">[9906: Homo sapiens (human) ](https://www.google.com/url?q=https://www.ncbi.nlm.nih.gov/Taxonomy/Browser/wwwtax.cgi?id%3D9606&sa=D&ust=1559232913848000)</span>
* <span class="c10">[10090: Mus musculus (house mouse) ](https://www.google.com/url?q=https://www.ncbi.nlm.nih.gov/Taxonomy/Browser/wwwtax.cgi?id%3D10090&sa=D&ust=1559232913849000)</span>
* <span class="c10">[10116: Rattus norvegicus (Norway rat) ](https://www.google.com/url?q=https://www.ncbi.nlm.nih.gov/Taxonomy/Browser/wwwtax.cgi?id%3D10116&sa=D&ust=1559232913849000)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 332.00px;">![](images/image10.png)</span>

<span class="c3"></span>

1.  <span class="c3">ここで、各遺伝子毎にLinked BioAssays Countが表示されています。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 264.00px; height: 48.00px;">![](images/image73.png)</span>

<span class="c3"></span>

1.  <span class="c3">Linked BioAssays Countのあとの数値、この場合は"12"をクリックすると、BioAssaysのサイトへ移動します。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 361.33px;">![](images/image51.png)</span>

<span class="c3"></span>

1.  <span class="c3">Linked BioAssays Countのあとの数値、この場合は"12"をクリックすると、BioAssaysのサイトへ移動します。</span>

* <span class="c3">BioAssay AID,&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;BioAssay Name, BioAssay Type の表示された表が表示されます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 86.67px;">![](images/image64.png)</span>

<span class="c3"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 36.00px; height: 41.00px;">![](images/image89.png)</span><span class="c3">をクリックすると、説明が表示されます。この機能はPubChemの色々なサイトにありますので、”これ何？”と思ったら、クリックしてみてください。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 172.00px;">![](images/image22.png)</span>

<span class="c3"></span>

1.  <span class="c3">右上のDownloadをクリックとCSV形式で取得することができます。ダウンロードしたCSV形式のファイルを開くと以下のようになります。</span>

<span class="c3"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 149.33px;">![](images/image15.png)</span>

<span class="c3"></span>

1.  <span class="c3">テーブルの”BioAssay AID”をクリックすると、以下のようなアッセイの詳細を見ることができます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 554.67px;">![](images/image28.png)</span>

<span class="c3"></span>

1.  <span class="c3">詳細ページには上図のようなことが記載されています。</span>

* <span class="c3">”Tested Substances:”を見ていただくと、”Active”と”Inactive”の件数がわかります。</span>

* <span class="c3">”Data table”をクリックすると下記のTableが表示されます。これは、ページをスクロールすることや、ページ右端の”CONTENTS”の”2 Data Table”をクリックすることでも同様に移動できます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 433.33px;">![](images/image47.png)</span>

<span class="c3"></span>

1.  <span class="c3">右上の”？”をクリックすると ここでも説明が表示されます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 126.67px;">![](images/image19.png)</span>

<span class="c3"></span>

1.  <span class="c3">Data Tableには様々な情報が登録されています。右上の”SORT BY”のプルダウンにより、Activity, Score, SID, CID</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 177.33px;">![](images/image108.png)</span>

<span class="c3"></span>

1.  <span class="c3">右上のDownloadをクリックとCSV形式で取得することができます。また、Data Tableのダウンロードでは、下図のようにALL, ACTIVE, INACTIVEをそれぞれ取得できます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 361.00px; height: 213.00px;">![](images/image107.png)</span>

<span class="c3"></span>

1.  <span class="c3">取得したCSV形式のファイルを開くと以下のようになります。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 208.00px;">![](images/image86.png)</span>

<span class="c3"></span>

1.  <span class="c3">Data Tableからのリンクは、SID, Activity, Entrez GeneIDから、それぞれのページに移動することができます。</span>
2.  <span class="c3">Data Tableの各列のSIDのSID（例えば：152153881）をクリックすると下図のようなページが表示されます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 114.00px; height: 277.00px;">![](images/image52.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 389.33px;">![](images/image48.png)</span>

<span class="c3"></span>

1.  <span class="c3">このページでは、Depositor CommentsやSIDに関するBiological Test Resultsを得ることができます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 645.33px;">![](images/image14.png)</span>

<span class="c3"></span>

1.  <span class="c3">Data Tableの各列のActivityのActive or Inactiveをクリックすると下図のようなページが表示されます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 91.00px; height: 194.00px;">![](images/image5.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 201.33px;">![](images/image76.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 253.33px;">![](images/image43.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 310.67px;">![](images/image74.png)</span>

<span class="c3"></span>

1.  <span class="c3">Data Tableの各列のEntrez GeneIDをクリックすると下図のようなページが表示されます。このページでは、遺伝子に関する各種情報を見ることができます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 82.00px; height: 216.00px;">![](images/image70.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 381.33px;">![](images/image49.png)</span>

---

<span class="c3"></span>

<span class="c3"></span>

### <span class="c42">URLへキーワード（遺伝子名、生物種など）を用いた検索</span>

* <span class="c3">以下のようなURLを用いることで、キーワードに該当するエントリーを表示させることもできます。</span>
* <span class="c10">[https://pubchem.ncbi.nlm.nih.gov/gene/ACADM/human](https://www.google.com/url?q=https://pubchem.ncbi.nlm.nih.gov/gene/ACADM/human&sa=D&ust=1559232913856000)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 350.67px;">![](images/image65.png)</span>

<span class="c3"></span>

* <span class="c10">[https://pubchem.ncbi.nlm.nih.gov/protein/P00533](https://www.google.com/url?q=https://pubchem.ncbi.nlm.nih.gov/protein/P00533&sa=D&ust=1559232913857000)</span>

<span class="c3"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 309.33px;">![](images/image13.png)</span>

<span class="c3"></span>

<span class="c19">PubChem Classification Browserを使ったデータ取得</span>
----------------------------------------------------------------

1.  <span class="c3">下記の検索ボックス下にあるアイコンの右から二番目の"Browse Data"をクリックします。</span>

* <span class="c3">または、下記のURLへ移動します。</span>

* <span class="c10">[https://pubchem.ncbi.nlm.nih.gov/classification/#hid=1](https://www.google.com/url?q=https://pubchem.ncbi.nlm.nih.gov/classification/%23hid%3D1&sa=D&ust=1559232913858000)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 321.33px;">![](images/image103.png)</span>

<span class="c3"></span>

1.  <span class="c3">下図のようなClassification Browserが表示されます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 334.67px;">![](images/image99.png)</span>

<span class="c3"></span>

1.  <span>Select classificationで、”</span><span class="c39">ChEMBL</span><span class="c3">”を選択してください。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 353.33px;">![](images/image42.png)</span>

<span class="c3"></span>

1.  <span class="c3">Data type counts to display の下に、None, Compound, Substance, Assay, PubMed, Gene, Protein, Taxonomy が表示されました。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 496.00px; height: 37.00px;">![](images/image94.png)</span>

<span class="c3"></span>

1.  <span class="c3">AssayやGeneを選択すると、以下のように項目に含まれる数値が変わります。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 663.00px; height: 319.00px;">![](images/image50.png)</span>

1.  <span class="c3">左の青三角をクリックすると下の階層が表示されます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 459.00px; height: 201.00px;">![](images/image34.png)</span>

1.  <span>右</span><span class="c3">の青い数字をクリックすると、リストが表示されます。 </span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 226.67px;">![](images/image27.png)</span>

<span class="c3"></span>

1.  <span class="c3">左上のプルダウンで、Format, 表示件数、ソートを変更できます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 187.20px; height: 208.70px;">![](images/image80.png)</span><span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 169.70px; height: 169.70px;">![](images/image93.png)</span><span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 256.40px; height: 149.70px;">![](images/image85.png)</span>

<span class="c3"></span>

1.  <span class="c3">左の Results by taxonから、生物種を選択して絞り込みができます。</span>

<span class="c3"></span>

<span class="c3"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 265.00px; height: 207.00px;">![](images/image102.png)</span>

<span class="c3"></span>

1.  <span>検索（選択）されたリストは右上の”Send to:”のプルダウンから、形式を選択してデータ得ることができます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 438.00px; height: 139.00px;">![](images/image21.png)</span>

<span class="c3"></span>

---

<span class="c3"></span>

<span class="c3"></span>

---

<span class="c3"></span>

<span class="c3"></span>

<span class="c14">5. ChEMBL</span>
==================================

<span class="c19">ChEMBLの説明</span>
----------------------------------

* <span class="c3">ChEMBLとは</span>

* <span class="c3">ChEMBLはEBIのChEMBLチームにより維持管理されている化合物の活性などを収録したデータベース</span>

* <span class="c3">以下のリンクも参考になります。</span>

* <span class="c10">[https://github.com/Mishima-syk/py4chemoinformatics/blob/master/ch04_database.asciidoc](https://www.google.com/url?q=https://github.com/Mishima-syk/py4chemoinformatics/blob/master/ch04_database.asciidoc&sa=D&ust=1559232913862000)</span>

<span class="c3"></span>

* <span class="c3">ChEMBL Interface Questions</span>

* <span class="c10">[https://chembl.gitbook.io/chembl-interface-documentation/frequently-asked-questions/chembl-interface-questions#can-i-edit-the-query-being-used](https://www.google.com/url?q=https://chembl.gitbook.io/chembl-interface-documentation/frequently-asked-questions/chembl-interface-questions%23can-i-edit-the-query-being-used&sa=D&ust=1559232913863000)</span>

<span class="c3"></span>

* <span class="c3">chembl-interface-documentation</span>

* <span class="c10">[https://chembl.gitbook.io/chembl-interface-documentation/](https://www.google.com/url?q=https://chembl.gitbook.io/chembl-interface-documentation/&sa=D&ust=1559232913864000)</span>

<span class="c3"></span>

<span class="c3"></span>

---

<span class="c3"></span>

### <span class="c42">ウェブブラウザを利用して</span>

1.  #### <span>ChEMBLのサイト（</span><span class="c10">[https://www.ebi.ac.uk/chembl/](https://www.google.com/url?q=https://www.ebi.ac.uk/chembl/&sa=D&ust=1559232913864000)</span><span class="c24 c21">）を開く</span>

* <span class="c3">または、Googleなどの検索エンジンで”ChEMBL”と検索し、下記のリンクをクリック</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 169.33px;">![](images/image71.png)</span>

---

<span class="c3"></span>

1.  #### <span class="c24 c21">概要</span>

##### <span class="c12 c21">含まれるデータの俯瞰</span>

* <span>左図の"</span><span class="c13"><</span><span>”, "</span><span class="c13">></span><span class="c3">"をクリックすると、表示される項目が以下のようにかわります。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 644.81px; height: 723.44px;">![](images/image101.png)</span>

<span class="c3"></span>

<span class="c3"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 404.00px;">![](images/image39.png)</span>

<span class="c3"></span>

---

<span class="c3"></span>

##### <span class="c12 c21">階層</span>

* <span class="c3">表示された項目をクリックすることで下の階層を見ることができます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 390.67px;">![](images/image61.png)</span>

<span class="c3"></span>

* <span class="c3">"Enzyme"をクリックすると下図（中央）のように下の階層を見ることができます。</span>
* <span class="c3">さらに"Kinase"をクリックすると下図（右）のように下の階層を見ることができます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 211.44px; height: 205.70px;">![](images/image91.png)</span><span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 200.50px; height: 189.70px;">![](images/image105.png)</span><span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 174.81px; height: 164.74px;">![](images/image90.png)</span>

---

<span class="c3"></span>

##### <span class="c12 c21">年代毎の分子の種類の分布</span>

* <span class="c3">マウスオーバーするとデータが表示されます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 528.00px; height: 431.00px;">![](images/image68.png)</span>

---

<span class="c3"></span>

##### <span class="c12 c21">Taxonomyによる分類</span>

* <span class="c3">クリックして中を見ていくことができます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 396.00px;">![](images/image11.png)</span>

---

<span class="c3"></span>

<span class="c3"></span>

##### <span class="c12 c21">開発フェーズとUSAN登録</span>

* <span class="c3">マウスオーバーして、クリックするとその情報が表示されます。</span>

<span class="c3"></span>

<span class="c3"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 298.67px;">![](images/image84.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 338.67px;">![](images/image114.png)</span>

<span class="c3"></span>

---

<span class="c3"></span>

##### <span class="c12 c21">病気のフェーズ</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 397.33px;">![](images/image75.png)</span>

* <span class="c3">色のついたところをクリックすると下図のような関連する化合物リストが表示されます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 304.00px;">![](images/image30.png)</span>

<span class="c3"></span>

---

<span class="c3"></span>

<span class="c3"></span>

##### <span class="c12 c21">化合物</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 269.81px; height: 270.68px;">![](images/image69.png)</span>

* <span class="c3">Compoundsをクリックすると下図のような化合物リストが表示されます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 508.00px;">![](images/image62.png)</span>

<span class="c3"></span>

---

<span class="c3"></span>

<span class="c3"></span>

#### <span class="c24 c21">機能の説明</span>

##### <span class="c12 c21">表示切り替え</span>

* <span class="c3">左上のTable, Card, Graph, Heatmapをクリックすると表示を切り替えることができます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 224.00px; height: 71.00px;">![](images/image104.png)</span>

##### <span class="c12 c21">絞り込み</span>

* <span class="c3">Filterから絞りたい項目をクリックして選択すると、データを絞り込むことができます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 342.00px; height: 520.00px;">![](images/image67.png)</span><span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 348.00px; height: 625.00px;">![](images/image33.png)</span>

* <span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 103.00px; height: 52.00px;">![](images/image3.png)</span><span class="c3">で、フィルターをクリアすることができます。</span>

##### <span class="c12 c21">データダウンロード</span>

* <span class="c3">右上のアイコンからダウンロートする形式を選んで選択したデータをダウンロードすることができます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 224.00px; height: 51.00px;">![](images/image1.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 425.33px;">![](images/image18.png)</span>

<span class="c3"></span>

---

<span class="c3"></span>

<span class="c3"></span>

#### <span class="c21 c24">アッセイ</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 269.81px; height: 270.68px;">![](images/image69.png)</span>

* <span class="c3">上図の"Assays"をクリックすると、下図のようなアッセイリストが表示されます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 328.00px;">![](images/image96.png)</span>

<span class="c3"></span>

* <span class="c3">左にある”Filters”で、各種条件でフィルターすることができます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 417.33px;">![](images/image60.png)</span>

<span class="c3"></span>

* <span class="c3">リストにある”ChEMBL ID”のリンクをクリックすると下図のような”Assay Report Card”が表示されます。</span>

* <span class="c3">Assay Report Cardには、Basic Information, Curation Summary, Activity Charts, Compound Summaryが含まれています。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 329.33px;">![](images/image56.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 124.00px;">![](images/image81.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 551.00px; height: 492.00px;">![](images/image16.png)</span>

* <span class="c3">Bioactivityでクリックすると、活性情報のリストが表示されます。</span>

<span class="c3"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 261.33px;">![](images/image26.png)</span>

<span class="c3"></span>

---

<span class="c3"></span>

<span class="c3"></span>

#### <span class="c24 c21">targets</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 269.81px; height: 270.68px;">![](images/image69.png)</span>

* <span class="c3">"Targets"をクリックすると、下図のようなリストが表示されます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 374.67px;">![](images/image20.png)</span>

<span class="c3">Organism: Homo Sapiens, Protein Classification L2: Kinase</span>

<span class="c3"></span>

* <span class="c3">左にあるFiltersを用いて、絞り込むことができます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 612.00px;">![](images/image17.png)</span>

<span class="c3"></span>

* <span class="c3">リストの"ChEMBL ID"をクリックすると、下図のような”Target Report Card”が表示されます。</span>

* <span class="c3">”Target Report Card”には、以下に示すような様々な情報が含まれています。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 417.33px;">![](images/image8.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 373.33px;">![](images/image63.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 481.33px;">![](images/image29.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 636.00px;">![](images/image40.png)</span>

<span class="c3"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 524.00px;">![](images/image55.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 314.67px;">![](images/image45.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 185.33px;">![](images/image54.png)</span>

<span class="c3"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 144.00px;">![](images/image97.png)</span>

<span class="c3"></span>

---

<span class="c3"></span>

<span class="c3"></span>

### <span class="c42">キーワード検索</span>

#### <span class="c24 c21">化合物・医薬品</span>

<span class="c3"></span>

<span class="c3">レキサルティ</span>

<span class="c3"></span>

<span class="c10">[https://www.kegg.jp/medicus-bin/japic_med?japic_code=00067274](https://www.google.com/url?q=https://www.kegg.jp/medicus-bin/japic_med?japic_code%3D00067274&sa=D&ust=1559232913877000)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 392.00px;">![](images/image110.png)</span>

<span class="c3">“Brexpiprazole”を検索してみましょう</span>

* <span class="c3">トップページ右上の入力欄にキーワードを入力します。今回は”Brexpiprazole”</span>

<span class="c3"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 105.33px;">![](images/image4.png)</span>

<span class="c3"></span>

* <span class="c3">キーワードを入力すると関連情報が表示されます。ここでは、  </span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 261.00px; height: 32.00px;">![](images/image12.png)</span>

<span class="c3">からCompoundsに含まれているデータであることがわかります。</span>

<span class="c3"></span>

<span>右下に表示される</span><span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 175.00px; height: 33.00px;">![](images/image41.png)</span><span class="c3">をクリックすると分子の詳細ページが表示されます。</span>

<span class="c10">[https://www.ebi.ac.uk/chembl/compound_report_card/CHEMBL2105760/](https://www.google.com/url?q=https://www.ebi.ac.uk/chembl/compound_report_card/CHEMBL2105760/&sa=D&ust=1559232913879000)</span>

<span class="c3"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 301.33px;">![](images/image77.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 212.00px;">![](images/image32.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 109.33px;">![](images/image109.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 272.00px;">![](images/image35.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 132.00px;">![](images/image53.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 384.00px;">![](images/image7.png)</span>

<span class="c3"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 349.33px;">![](images/image95.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 258.67px;">![](images/image38.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 321.33px;">![](images/image59.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 558.67px;">![](images/image83.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 370.67px;">![](images/image111.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 225.33px;">![](images/image82.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 569.33px;">![](images/image37.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 528.00px;">![](images/image58.png)</span>

<span class="c3"></span>

<span class="c3"></span>

<span class="c3"></span>

#### <span class="c24 c21">遺伝子名</span>

* <span class="c32">MAPK6</span><span class="c3">遺伝子</span>

<span class="c3">ヒトでマイトジェン活性化プロテインキナーゼ6をコードするMAPK6遺伝子</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 94.67px;">![](images/image46.png)</span>

<span class="c3"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 220.00px; height: 37.00px;">![](images/image9.png)</span>

<span class="c3">からTargetsに含まれていることがわかります。</span>

<span>右下に表示される</span><span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 147.00px; height: 34.00px;">![](images/image88.png)</span><span>をクリックすると</span><span class="c10">[詳細ページ](https://www.google.com/url?q=https://www.ebi.ac.uk/chembl/target_report_card/CHEMBL5121/&sa=D&ust=1559232913882000)</span><span class="c3">へ移動します。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 253.33px;">![](images/image92.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 154.67px;">![](images/image106.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 362.67px;">![](images/image113.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 430.00px; height: 504.00px;">![](images/image87.png)</span>

<span class="c3"></span>

* <span class="c3">ここで、マウスカーソルをKdにのせて、クリックすると詳細データが表示されます。</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 390.67px;">![](images/image72.png)</span>

<span class="c3"></span>

<span class="c3"></span>

<span class="c3"></span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 488.00px;">![](images/image31.png)</span>

* <span class="c3">各プロットにマウスカーソルをのせると、プロットの情報が表示されます。</span>

<span class="c3"></span>

<span class="c23">BEI / Binding Efficiency Index / 結合効率指数</span>

<span class="c23">SEI / Surface-binding Efficiency Index / 表面結合効率指数</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 474.67px;">![](images/image112.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 616.00px;">![](images/image23.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 518.67px;">![](images/image79.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 313.33px;">![](images/image36.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 188.00px;">![](images/image44.png)</span>

<span style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 680.61px; height: 140.00px;">![](images/image57.png)</span>

<span class="c3"></span>

---

<span class="c3"></span>

<span class="c3"></span>

<span>付録：</span><span class="c35 c32 c40">ドキュメント作成手順</span>
===========================================================

1.  <span class="c3">Google Documentで内容作成</span>
2.  <span class="c3">Google Documentの”ファイル”→”形式を指定してダウンロード”で、”ウェブページ(html)”を選択する。</span>
3.  <span class="c3">ダウンロードしたzipファイルを解凍する。</span>
4.  <span class="c3">HTML - Markdown 変換</span>

1.  <span class="c10">[https://pronama.jp/md/](https://www.google.com/url?q=https://pronama.jp/md/&sa=D&ust=1559232913886000)</span>

1.  <span class="c3">Githubへhtmlとmdファイル、必要な画像ファイルをアップロード</span>

<span class="c3"></span>

<span class="c3"></span>

<span class="c3">以上</span>

<span class="c3"></span>

<span class="c3"></span>

<span class="c3"></span>

<div>
    <span class="c3"></span>
</div>
