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

