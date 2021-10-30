# kaggle_diary
about kaggle_diary  

RSNA-MICCAI Brain Tumor Radiogenomic Classificationについて　　

## 20210918
【Brain Tumor】EDA for starter(日本語version)[~url~](https://www.kaggle.com/chumajin/brain-tumor-eda-for-starter-version) をみて、コンテストの内容を少しだけ把握した。  
先は厳しそう  
[TF] Simple Prediction with VGG16 (日本語)[~url~](https://www.kaggle.com/masatomurakawamm/tf-simple-prediction-with-vgg16)を途中まで読み進めた。  
デコレータについて少し勉強した。直接は関係ないけど。  

## 20210919
[TF] Simple Prediction with VGG16 (日本語)[~url~](https://www.kaggle.com/masatomurakawamm/tf-simple-prediction-with-vgg16)をやってみた。  
0.368が出たね。完全にコピペだけどね。  

## 20210920
[TPU] RSNA Keras 3D CNN Voxel Train [~url~](https://www.kaggle.com/sreevishnudamodaran/tpu-rsna-keras-3d-cnn-voxel-train)をちょっと読んでみる
 TPUで警告が出たからkaggleのnotebook上でやるのは厳しいようだ
 すごそうだけど、最初のとこしか読めてないから、configがパラメータの設定であることや、データの読み込みのとこくらいしかわからんかった。
 
## 20210921
昨日の続きを読んでた  
やっぱり銀メダル取る人はすげーや。みたことあるコードで喜んでるけど、ほとんどわからん。  
TPUを使ったコードを提出するのは難易度が高いから、ただコピペして提出するだけでも大変なんだなと思った。  
もっとたくさん読んで勉強していきたい。

[RSNA-MICCAI] Monai - ensemble[~url~](https://www.kaggle.com/mikecho/rsna-miccai-monai-ensemble)を読む。なんかシルバーのメダルついてる人のやつ。この人の参考資料みたいなのも後で読みたい。 
コードがめっちゃ綺麗だし、できそうな雰囲気もちょっとするし、すげえなこれ。

## 20210922
昨日のmonaiのやつを読み進めてた。コード実行したけど、処理長すぎてほんとに終わる気がしない。epochが16もあるのに4時間でepoch2も終わってない。　　
DenceNetとResNetの違いを学んだ。どちらも層を深くするためのモデルらしい。層が何百とかになってる。そら終わらんわ。  
処理重いし、解読も難しいから、他のnotebook行こうと思う。  
[使用notebook:monai_silver]  
Efficientnet3D with one MRI typeを読み進める。[~url~](https://www.kaggle.com/rluethy/efficientnet3d-with-one-mri-type)  
この辺からkaggleのnotebookが動かなくなった。

## 20210923  
昨日のEfiicientnet3Dのコードをいまだに読み解いてる。  
need at least on array to stack の謎がいまだに解けない。  
やばすぎる。

## 20210924  
Efficienetの3Dのコードの解読の続きをした。大体エラーが起こったところらへんまでたどり着いたけど、なんでそれが定義されてるのか全くわからんところがあった。  
だからそのnotebookに書いてあった参考資料を辿ることにした。  
🔥torch EfficientNet3d for 🧠 MRI [no 🌐][train]🔥[~url~](https://www.kaggle.com/furcifer/torch-efficientnet3d-for-mri-no-train)  
を読み進めて行こうと思う。  

## 20210925  
torch EfficientNet3d の方を進めた。  
まだdicom2arrayのところ。このnotebookにはnp.stackがなさそうだから、とりあえず動きそう。 
コードを確認しつつ、色々試していきたい。

## 20210926  
前回の続きを進めた。  
dicom2arrayについてとload_3d_dicom_imagesについて少しづつ理解できるようになった。  
転移学習とファインチューニングについても少しだけ学んだ。  
転移学習は学習済みモデルに対して出力そうのパラメーターを変えるもので、ファインチューニングは全ての層の中でパラメーターを微調整するものである。 

## 20210927
前回のコード解析を続けた。  
3時間くらいずっと学習をさせていてできたのだが、予測の仕方がわからずにせっかく出した重みも消えてしまった。  
そろそろ予測精度は出してみたいと思って、EfficientNet3d for 🧠 MRI[~url~](https://www.kaggle.com/xuxu1234/efficientnet3d-for-mri)  
を参考にしてpredictをしてsubmissionしようと思う。  
今日出せなかったものとコードは似ているから、もう一回挑戦すればできるかもしれない。

## 20210928  
今日はcodeで一番成績の良い人のnotebookを見た。🧠Brain Tumor 3D blender[~url~](https://www.kaggle.com/ammarnassanalhajali/brain-tumor-3d-blender)  
これは4つの予測結果に重みをつけてブレンドしてるらしい。  
ってことはこれを実現するには、その前の予測結果を出している部分についてみる必要がありそうだ。  
この人は4つのnotebookを作っているっぽい。  
🧠Brain Tumor 3D [EDA][~url~](https://www.kaggle.com/ammarnassanalhajali/brain-tumor-3d-eda)  
🧠Brain Tumor 3D [Inference][~url~](https://www.kaggle.com/ammarnassanalhajali/brain-tumor-3d-inference)    
🧠Brain Tumor 3D [Training][~url~](https://www.kaggle.com/ammarnassanalhajali/brain-tumor-3d-training)   
これを一個一個見ていこうと思う。  
まずはEDAから読み進めていく。

## 20210929  
今日は pocketさん『猫でも取れる金メダル & 猫しか取れない金メダル』- Kaggle meetup Tokyo #4　[~url~](https://www.youtube.com/watch?v=6DW5PCIo5qc)  
を視聴した。discussionを見ることは意外に重要なんだなと思った。重要なところに絞ってやることを頑張っていきたい。行き詰まってきた今だからこそ。

## 20210930  
段々自分でコードが書けない、エラーが出まくるコンペがキツくなってきた。学習的無力感的なやつかな。もう名前もはっきり覚えていないけど。  
本当は最後まで気力で押し通そうと思ってたけど、この辺は撤退して、できそうなコンペで一旦自信を付け直すのもありかなと思ってきた。  
だから他のコンペに移ります。  

Google Brain - Ventilator Pressure Prediction
ここからは別のコンペの「人工呼吸器の圧力の予測」に移ります  
Ventilator Pressure Prediction: EDA, FE and models[~url~](https://www.kaggle.com/artgor/ventilator-pressure-prediction-eda-fe-and-models)  
まずはこれで今回のコンペの内容を少しだけ学んだ。  
時系列データっぽいけど回帰の問題なんだなってことや人工呼吸器のシュミレートをして、呼吸中の呼吸回路の気道圧力を正しく予測するものなんだなって知った。  
あと、discussionにstarterのためのnotebookをまとめてくれてるところがあったからそこも拝見した。  
[Compilation] Good starter notebooks[~url~](https://www.kaggle.com/c/ventilator-pressure-prediction/discussion/275039)  

## 20211001  
昨日のやったLightAutoML[~url~](https://www.kaggle.com/tsano430/lightautoml-starter)の模写で、スコアが0.284でた。多分10時間くらい動かせば0.244出たんだろうけど一時間だけだからこれくらいかなって感じ。その人にコメントしたらもっといいnotebook紹介してもらったから、そっちもみてみようと思う。

## 20211002  
今日は前回教えてもらった改善版を動かしていく。  
LightAutoML + Bidirectional LSTM[~url~](https://www.kaggle.com/tsano430/lightautoml-bidirectional-lstm)  
ってやつなんだけど、これを作るためにはImprovement base on Tensor Bidirect LSTM (0.173)[~url~](https://www.kaggle.com/tsano430/improvement-base-on-tensor-bidirect-lstm-0-173)  
で作ったファイルが必要みたいだから、これも動かしていく。  
codeやdiscassionを動かしてみながらも、自分でモデルを作ったりも進めていきたいなと思っている。
 
## 20211003  
今回も前回の続きをやる  
並行しながら、Ensemble Folds with MEDIAN - [0.153][~url~](https://www.kaggle.com/cdeotte/ensemble-folds-with-median-0-153)  
この人のnotebookも進めてた。 cupyとcudfが出てきてびっくりしたけど、gpuのときに使えて、高速で動くnumpyとpandasみたいなものらしい。  
全然cupyが入らなくて大変だと思ったけど、結局acceleratorがGPUになっていなかったことが問題だった。それだけかぁと思ったけど、ライブラリによっては入るものと入らないものがあるのだと知って、勉強になった。あと、pip installのときに-yを入れるとショートカットできるの地味にいいな。

## 20211004  
前回の続きをがんばります。  
discussionを2つくらい読んだ。forkすればいいんだろうけど、如何せん処理が長すぎて萎えてる。  
別のやり方を考えたほうがいいかもしれない。それこそkaggleとかのほうがいいのか。  
環境について勉強したほうが、forkするのも楽になるから、その辺も同時並行で進めていきたい。  

## 20211005  
今日はgooglecolabでkaggleのデータ持ってきて動かそうと思ったんだけど、データのダウンロードがまぁうまくいかない。  
まじで萎えてた。dataのuploadの仕方もわからんし、裏で回せないしで、正直行き詰まっているというか。  
うまくいかなくてやる気がめちゃくちゃ削がれている感じ。  
成果でない、やり方もわかるわけじゃないってところでぐるぐるしてる。discassion読んで、できそうなところは工夫しながらやるって形で、粘っていきたいと思う。  
新しい開発環境については、勉強というか知識が圧倒的に足りないだろうから、ちょっとずつ広げていく形でやっていきたい。  
googlecolabはそろそろ使えるようになりたいから、少しづつやって行こう

## 20211006  
そろそろやる気が削がれてきたから、もう少し計画を見直そうかなと思った。daigoの動画を見て、目標を立てることのデメリットは目の前のことに集中できなくなるかららしい。  
確かに、結果を早急に求めて、本来まだ少し遠いはずのところに急いで行こうとしてた。そのせいか、目の前のことに集中できなかったし、できないことを一つづつ乗り越えるということも少しづつできなくなっていた。目標は遠くても、焦らず、チャンスを狙いながら、じっくり、リラックスして取り組めるように変えていこうと思う。  
ちなみに今回はkaggleのmashinelearningのintroでリハビリしたのと、Ventilator Pressure simple EDA[~url~](https://www.kaggle.com/currypurin/ventilator-pressure-simple-eda)を見ながら、一歩一歩データを動かしていった。焦らず、自分のできる範囲で動かしながら、少しづつレベルアップしていこう。  

## 20211007  
今日はほぼ何にもできんかったね。EDAを少しだけやってコピって、カウントエンコーディングをちょっと試したくらい。  
discassionを3つほど読んだ。なんか日本人の人もそこそこいるんだなと思った。アンサンブルをやるためにはさまざまなモデルを試した方がいいらしい。  
これいろんなコンペに当てはまることだから、色々準備しておけば次の時も使えるよな。  
今日はこんなとこで。少しづつ続けていこう。

## 20211008
discassionを二つほど見た。特徴量を作るときに色々試行錯誤しているのだと知って、自分も色々試してみようと思った。  

## 20211009  
LSTMとBILSTMを少し学ぼうと思った。[Compilation] Good starter notebooks[~url~](https://www.kaggle.com/c/ventilator-pressure-prediction/discussion/275039)    
を参照して、LightAutoML Continuer :)[~url~](https://www.kaggle.com/alexryzhkov/lightautoml-continuer)  
を見ながらやっていこうと思う

## 20211010  
LSTMについて勉強していた。Youtubeで解説動画見てたけど、まだ、 lstmって普通のディープラーニングより過去の情報を持って置けるってことくらいしかわからない。だからどうやって使うのかこれからもうちょっと知っていきたい。

## 20211011  
LSTMの勉強を引き続き続けた。

## 20211012
LSTMを何とか実装しようと頑張った

## 20211013
LSTMをsignateの方で何とかたどり着いたけど、kaggleでやっていることとの整合性が全く取れなくなり、振り出しに戻ったような感覚になった。  
一旦LSTMはストップしておこうかと思っている。signateで意外と沼にハマっていて抜け出せない。

## 20211014
discussionを読んで、回帰問題を分類問題として見るものがあるのだと知った。

## 20211015
discussionを読んで、fold数について学んだ。確かに5foldよりも10foldの方が単体のモデルでは評価が高まるかもしれないが、実際は5foldで二つのモデルを試した方が時間的にはいいのだとわかった。

## 20211016
注意深くdiscussionを読んでcodeを直せば銀の中間くらいにいけるらしい。大事なのはまず発想力じゃない。基礎的なことを学ぶ能力とコードの内容を紐解ける能力と、学習の時間をどうやって取るかっていうことだけだ。

## 20211017
なんかpytorchのコード載ってたけど、もしかしたらちょっと読めそうかなと思った。PyTorch LSTM with TensorFlow-like initialization[~url~](https://www.kaggle.com/junkoda/pytorch-lstm-with-tensorflow-like-initialization/notebook)  
SELUとかいうRELUの負の値も取れるバージョンもあるんだって。すごいね。まだまだ知らないことがたくさんある。

## 20211018
よっしゃdiscussion読むぞ  
時間がかかる問題がやっぱりあるらしくて、インタラクティブにやる方法だったり、オンラインのコンピュータを借りる方法だったり色々あるらしい。　
この辺の環境構築についても学んでいけたらもっと楽しくなりそうな気もしている
モンテカルロドロップアウト法っていうのがあるんだね。知らんかった。  
これからも細く長く続けていきたい。

## 20211019
今日は久しぶりにコードを動かした。今日LAIMEの運営の人に聞いたけど、自動で動かすにはkaggleのnotebookが最適らしい。それ以外だったらcolabpro+を使う必要があるんだって。  
これでやっとできると思うと嬉しい。同時に色々できそうだ。

## 20211020
前回動かしていたnotebook見てみたけど、全然できてなかったね。ただ動かして提出するだけでもコードの書き方色々あるんだろうな。その辺も勉強していけたらなと思う。  
桁数を増やしてみてはいかがかという主催者に対しての要望がdiscussionにあった。そんな提案もすることもあるんだなぁ。

## 20211021
今日はLAIMEのかぐるべんきょーかいに参加した。医療系で頭いい人がいっぱいいた気がした。kaggleで銀は目指しているところでもあるから、
レベル感がわかってよかった。画像分析で途中から入ったから詳しくはわからなかったけど、すごいと思った。負けじと頑張りたい。

## 20211023
kaggle日記を続けて1ヶ月が経つ。昨日は1日スキップしちゃったけど、細く長く続けていこう。
tpu使うときにfloat64よりもfloat32の方が早く済むらしい。知らんかった。

## 20211025
forkしたけど全然結果出ないやつだった。  
ちゃんと見てやる必要がありそう。

## 20211026
discussion見てたけど、時系列分析でtransformerやるやつがあるらしい。  
なんかすごそうだけど全然使えなさそう  
LAIMEのプライベートコンペ面白そうだからちょっとやってみる。

## 20211027  
なんかtransformerで多変量時系列分析やるってすごいな  
教師なしって言ったたしバケモンじゃん。
スコアの高すぎるnotebook出すと警告出るらしい  
俺には関係ないかもだけど。

## 20211028
アンサンブルをするときに、中央値や平均値を使うことが多いが、そうではなく、分布の形を見て 
判断するものもあるらしい。アンサンブルも奥が深いんやな。

## 20211029  
コンペの最終日になるといろんな人が上を目指し本気でやる中でなるべく高いスコアを出そうとズルのようなことをする人もいるし、モチベーションの低下や他のすごい人の解決法を見たいといい、メンターシップをお願いする人もいる。  
みんな精度が出ない中辛い道を進み続けている。  
これがkaggleの道。なかなか厳しいね。けどやってやりたいと思う。  
結果は確かに大事。最初のモチベはそこから。だけど見失っちゃいけない。  
結果が出るのは実力がある程度ついてるから。確かにショートカットの方法もあるかもしれない。賢くいけば考えなくてもいいのかもしれない。だけど、少しずつやっていこう。  
一番欲しいのはメダルじゃない。メダルを取れる実力だ。

## 20211030
ニューラルネットをトレーニングするときにもいくつかコツがあるらしい。  
そんなに使ったことがないからわからないけど。今度やるときはそういうのも見てみようかな。

