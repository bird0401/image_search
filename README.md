# image_search
## dataset
- [CelebA Dataset](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html)

## tips
- crop background using semantic segmentation

## reference
### code
- [深層距離学習(Deep Metric Learning)の基礎から紹介](https://tech-blog.optim.co.jp/entry/2021/10/01/100000#ArcFace)
  - metric learning can take discriminative feature vector
  - contrasive approach
    - compare sample pair
    - how to take pairs is important
    - tripet loss
  - softmax approach
    - reuse class labels
    - cant do in none class label case
    - arcface
- [類似画像検索ツールを作ってみる (1) 序章](https://zenn.dev/kleamp1e/articles/202105-similar-search-1)
  - not using contrasive loss
  - model : MovileNet V2
- [画像検索に使用できるMetric LearningをGoogle Colabで試してみた](https://www.yurui-deep-learning.com/2021/01/19/%E7%94%BB%E5%83%8F%E6%A4%9C%E7%B4%A2%E3%81%AB%E4%BD%BF%E7%94%A8%E3%81%A7%E3%81%8D%E3%82%8Bmetric-learning%E3%82%92google-colab%E3%81%A7%E8%A9%A6%E3%81%97%E3%81%A6%E3%81%BF%E3%81%9F/)
  - ShamNetwork
- [metric learningで人間並みのアニメキャラ識別性能を目指す！](https://toa-hakobune.hatenablog.com/entry/2021/01/11/212459)
  - anime face 
  - segmentation
  - various metric learning approach
### PyTorch Metric Learning 
- [PyTorch Metric Learning](https://kevinmusgrave.github.io/pytorch-metric-learning/)
  - official doc
- [距離を近づけろ！Pytorch Metric Learningで始めるDeep Metric Learning](https://qiita.com/dcm_ishii/items/4abb2f0090c43b293cb1)
- [PyTorch Metric LearningによるDeep Metric Learningの実践](https://tech-blog.optim.co.jp/entry/2022/04/06/100000)
### outline
- [類似画像検索の3つの手法と精度向上のテクニック](https://www.imagazine.co.jp/%E9%A1%9E%E4%BC%BC%E7%94%BB%E5%83%8F%E6%A4%9C%E7%B4%A2%E3%81%AE3%E3%81%A4%E3%81%AE%E6%89%8B%E6%B3%95%E3%81%A8%E7%B2%BE%E5%BA%A6%E5%90%91%E4%B8%8A%E3%81%AE%E3%83%86%E3%82%AF%E3%83%8B%E3%83%83%E3%82%AF/)
  - akaze:use for feature matching
  - segmentation may lead higher accuracy
- [コード解剖!! <深層距離学習 ArcFace>](https://qiita.com/kanataken/items/9b6af8f5c703ed0e21e0)
- [距離学習（Metric Learning）入門から実践まで](https://cpp-learning.com/metric-learning/#Metric_Learning-2)
  - mmc supervised
- [Facebook AI主催の画像のコピー検知のコンペで入賞した際の取り組み](https://engineering.dena.com/blog/2021/12/fb-isc-1st/)
  - contrasive loss
  - cross batch memory
  - use pytorch metric learning library
  - gem pooling
- [Deep Metric Learningによる、ホテルや飲食店などの拠点検索改善](https://techblog.yahoo.co.jp/entry/2021120330233760/)
  - metric learning to text feature
  - contrasive
  - producting using tensorflow serving
### serving
- [Tensorflow Serving を使い倒す](https://qiita.com/cvusk/items/abe68076bbbb87966539)
- 

### others
- [metric learning のファッション分野における活躍](https://zenn.dev/hrsma2i/articles/metric-learning-adcal-20-22)
  - deep learning for fashion
  - text to image
