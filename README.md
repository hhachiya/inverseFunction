### 武将データの可視化ツールの実行方法
### 要件
* Ubuntu 16.04
* Anaconda python 3.6（Scikit-learn, numpy, matplotlibなどの標準的なパッケージ込み）

### 実行例
以下のようにanalyze_warrior.pyを実行すると、T-SNEで次元削減しクラスタリングされた武将データの２次元プロットと、各クラスターに関連する語、および各クラスターに属する武将名の一覧を表示することができます。。

python analyze_warrior.py
 
![alt text](https://raw.githubusercontent.com/hhachiya/invereFunction/master/analysis_cluster.png "clustering result")

```python
Enterを押すと, 各クラスター中心に関連する語top5を表示します
クラスター0 (-2.4,-8.9): ['高房', '重政', '主膳', '忠光', '忠重']
クラスター1 (6.6,5.8): ['眞廣', '舂屋', '眤', '成願', '本阿弥']
クラスター2 (-5.4,-3.0): ['主君', '老臣', '旧臣', '輝元', '義宣']
クラスター3 (1.4,7.8): ['百姓', '不届き', '説諭', '妻女', '乞い']
クラスター4 (9.1,1.9): ['家来', '饗する', '忙然', '眞廣', '高房']
クラスター5 (-8.9,-9.6): ['城主', '長秀', '家臣', '信実', '隆信']
クラスター6 (1.5,-4.3): ['高房', '主君', '旧主', '老臣', '信綱']
クラスター7 (5.1,-0.5): ['老臣', '家康', '主君', '旧主', '出奔']
クラスター8 (-2.0,2.6): ['老臣', '主君', '旧主', '父子', '元親']
クラスター9 (6.8,12.2): ['信実', '細川幽斎', '宗長', '藤長', '眞廣']

Enterを押すと, クラスター0に属する武将一覧を表示します:
['井伊直宗' '井伊直元_(戦国時代)' '臼杵鎮続' '大槻太郎左衛門' '岡本保忠_(新助)' '蒲生重郷' '櫛橋伊家' '斎藤市郎左衛門'
 '斎藤徳元' '斎藤義興' '佐藤昌信' '真田幸隆' '白神果春' '武田信豊_(甲斐武田氏)' '水野忠政' '三好長逸' '伊達輝宗'
 '大友義鎮']


Enterを押すと, クラスター1に属する武将一覧を表示します:
['有馬豊氏' '宇喜多秀家' '織田信行' '加藤清正' '蒲生氏郷' '黒田長政' '小早川秀秋' '佐藤忠能' '真田信繁' '伊達成実'
 '津軽為信' '富樫晴貞' '徳川秀忠' '豊臣秀次' '豊臣秀保' '鳥居忠吉' '内藤忠興' '直江兼続' '中条藤資' '保科正光'
 '細川忠興' '前田利益' '松永久秀' '水野勝成' '三好実休' '三好之長' '柳生宗厳' '北条氏康' '今川義元' '北畠具教'
 '上杉謙信' '伊達政宗' '龍造寺政家' '武田信玄' '最上義光' '徳川家康']


Enterを押すと, クラスター2に属する武将一覧を表示します:
['朝倉景鏡' '跡部勝資' '雨森清定' '伊勢貞興' '猪俣邦憲' '大久保忠佐' '大熊朝秀' '織田信忠' '加賀井重望' '梶田直繁'
 '兼重元宣' '蒲生定秀' '蒲生秀行_(侍従)' '河尻秀隆' '福島正成' '斎藤利三' '相良武任' '陶晴賢' '瀬戸方久' '多賀常則'
 '津田信澄' '内藤弘矩' '鍋島直茂' '北条氏規' '本城惣右衛門' '本庄長英' '真柄隆基' '松平信康' '三好義興' '山口重勝'
 '吉岡長増' '斎藤義龍' '上杉憲政' '尼子義久' '朝倉貞景_(9代当主)']


Enterを押すと, クラスター3に属する武将一覧を表示します:
['明智光秀' '伊集院忠棟' '今村正実' '織田信孝' '北原兼孝' '吉川元長' '柴田勝家' '関口氏経' '宗義智' '武田義統'
 '三好為三' '山中勝重' '筒井順慶' '一条兼定' '北条氏政' '斎藤龍興' '伊東義祐' '大村純忠' '那須高資' '大内義隆'
 '織田信長' '宇都宮成綱']


Enterを押すと, クラスター4に属する武将一覧を表示します:
['尼子誠久' '一条信龍' '大久保長安' '加藤嘉明' '可児吉長' '栗山利安' '島津豊久' '島津義弘' '十河一存' '立花道雪'
 '立花宗茂' '中馬重方' '長宗我部信親' '豊臣秀長' '長野業正' '二宮就辰' '延沢満延' '益子勝宗' '松平忠吉' '松平康長'
 '三宅長盛' '村上義清' '森長可' '森成利' '山中幸盛' '尼子経久' '南部晴政' '島津義久' '相馬顕胤' '毛利元就']


Enterを押すと, クラスター5に属する武将一覧を表示します:
['朝比奈信置' '穴山信友' '井伊直満' '井伊直義' '石亀政頼' '板垣信憲' '海野昌雪' '岡部貞綱' '奥山朝忠' '奥山朝利'
 '小河信章' '長船定行' '小田氏治' '小野朝直' '小野朝之' '小野政直' '小山田行村' '梶田繁政' '上泉秀綱_(主水佐)'
 '京極高次' '小寺則職_(戦国時代)' '斎藤利堯' '関盛信' '高梨内記' '竹田津鎮満' '土岐定政' '中野直由' '鍋島忠茂'
 '林秀貞' '北条氏照' '堀田興重' '松田直長' '水野忠分' '武藤安成' '室賀久太夫' '武田信虎' '伊達晴宗' '佐竹義昭'
 '松前慶広']


Enterを押すと, クラスター6に属する武将一覧を表示します:
['浅野幸長' '井伊直孝' '伊木忠次' '色部光長' '大久保忠隣' '大庭三左衛門' '鬼庭綱元' '各務元正' '片倉景綱' '黒田一成'
 '斎藤利治' '佐伯惟治' '真田信尹' '島津忠恒' '下方貞清' '長連龍' '戸沢盛安' '豊臣秀吉' '塙直之' '堀直政' '本庄繁長'
 '本多正重' '宮田光次' '毛利秀包' '山岡重長' '山崎片家' '蘆名盛氏' '北条氏直' '山名政豊' '相良晴広' '松平清康'
 '相馬義胤_(十六代当主)' '北畠具房']


Enterを押すと, クラスター7に属する武将一覧を表示します:
['井伊直政' '池田輝政' '市橋長勝' '大谷吉継' '織田信雄' '金森長近' '蒲生賢秀' '黒田孝高' '高力清長' '後藤信康'
 '小早川隆景' '酒井忠次' '榊原康政' '坂崎直盛' '真田信之' '滝川一益' '竹中重治' '田中吉政' '谷衛友' '長宗我部盛親'
 '土井利勝' '藤堂高虎' '橋本一巴' '一柳直末' '平岩親吉' '福島正則' '堀秀政' '堀尾吉晴' '本多重次' '本多忠勝'
 '本多正純' '本多正信' '前田利家' '村田吉次' '毛利輝元' '毛利秀元' '山田宗昌' '山家公頼' '上杉景勝' '山名豊国']


Enterを押すと, クラスター8に属する武将一覧を表示します:
['朝倉宗滴' '尼子国久' '岩室重休' '飯富虎昌' '柿崎景家' '柏山明助' '河田長親' '北条高広' '香宗我部親泰' '陶興房'
 '高橋紹運' '団忠正' '富田長繁' '丹羽長秀' '穂井田元清' '北条氏邦' '北条綱成' '前田玄以' '三井弥一郎' '三好長慶'
 '森可成' '毛利隆元' '織田信秀' '佐竹義重_(十八代当主)' '朝倉義景' '尼子晴久' '島津貴久' '相良義陽' '宇喜多直家'
 '菊池義武' '里見義堯' '六角定頼' '大友義統' '筒井定次' '朝倉孝景_(10代当主)']


Enterを押すと, クラスター9に属する武将一覧を表示します:
['朝倉景紀' '安宅冬康' '板部岡江雪斎' '今川氏真' '大井信達' '蒲生貞秀' '菅正利' '北信愛' '吉川経基' '斎藤利綱'
 '斎藤妙椿' '佐川田昌俊' '佐野昌綱' '仙石久勝' '太原雪斎' '蜂須賀家政' '蜂屋頼隆' '北条幻庵' '細川幽斎' '三浦為春'
 '吉弘統幸' '脇坂安治' '六角義賢' '秋田実季' '畠山義綱' '大内義興' '宇都宮忠綱' '細川成之']
 ...
 ```

### word2vecとT-SNEを用いたライブドアのニュース記事の可視化

### 概要
ライブドアのニュース記事ごとに、ドキュメント特徴量を抽出します。
ドキュメント特徴量の抽出方法：
1. 記事に出現する単語のword2vec特徴量の平均


### 要件
* Ubuntu 16.04
* python 3.6

### インストール方法

#### Mecab
以下を参照して、インストールします。
http://hirotaka-hachiya.hatenablog.com/entry/2017/10/05/130026

#### word2vec
1. pip install gensim

#### livedoor-news-data
ライブドアのニュース記事データのtgzファイルをダウンロードし、livedoor-news-dataに置き、解凍します。
ライブドアのニュース記事は、カテゴリごとにxmlで記載されています。
1. cd livedoor-news-data
2. wget https://www.rondhuit.com/download/livedoor-news-data.tar.gz
3. tar -xvzf livedoor-news-data.tar.gz
4. cd ..

### 使い方
上記のインストールが完了した状態で、以下のようにword2vec_livedoor.pyを実行します。 

python word2vec_livedoor.py tfidf T F T

word2vec_livedoor.pyの引数は、
* 抽出方法(方式1:'w2v',方式2:'tfidf')
* 記事データへの処理を行うフラグ
* 辞書データの作成・更新を行うフラグ
* word2vecモデルの学習を行うフラグ
となっています。

### 各ニュースカテゴリに対する処理（方式１の場合）の説明
1. livedoor-news-dataからxmlの記事データを読み込む。
2. titleとbodyアイテムの値を抽出したテキストデータを、記事ごとに１行ずつlivedoor-news-data-txtに書き出す。
3. テキストデータにMecabで形態素解析し、形態素ごとに半角スペースで区切った形態素データをlivedoor-news-wakatiに書き出す。
4. 形態素データに対し、word2vecをかけて、記事ごとに平均を取ったベクトル（100次元）をlivedoor-news-pklに書き出す。つまり、pklには、記事の数 X 100次元の行列が保存される。

### 各ニュースカテゴリに対する処理（方式２の場合）の説明
1. livedoor-news-dataからxmlの記事データを読み込む。
2. titleとbodyアイテムの値を抽出したテキストデータを、記事ごとに１行ずつlivedoor-news-data-txtに書き出す。
3. テキストデータにMecabで形態素解析し、形態素ごとに半角スペースで区切った形態素データをlivedoor-news-wakatiに書き出す。
4. 形態素ごとに'形態素','全記事での出現回数','出現した文章の数','idf値'のデータフレームを作成、dataにcsv形式で書き出す。
5. 形態素データに対し、tf値を求める。同時にword2vecをかけて、形態素ごとのベクトル（100次元）にTF-IDF値をかけ合わせたものを記事ごとに平均したものをlivedoor-news-pklに書き出す。つまり、pklには、記事の数 X 100次元の行列が保存される。

