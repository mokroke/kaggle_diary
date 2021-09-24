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

