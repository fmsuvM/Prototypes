# MySun  

## Purpose  
ドローンに照明を乗せて，被写体を照らす撮影支援．  

## System  
被写体の周囲の平面を認識して，照らして欲しい場所をタッチしてドローン照明を向かわせる．そして撮影．  

![Plane Detection](https://gyazo.com/9cc6a7d2b9ff7532fbb0bb9cd2e7aa40.png)  
![Touch two points](https://gyazo.com/9633fb7dfac6c9cbd93ecb1c72d334ca.png)  
![Calibration](https://gyazo.com/1fed375c89fa0e1e64ee11ccb92dfa2f.png)  
![Touch Lighting Point](https://gyazo.com/b5c7eabbc555c8f1cdf33f621a5242b7.png)  
![Dlone Viewing](https://gyazo.com/21c5c0899df5cecec4517be12c636f14.png)  

## このアイディアの良いところ  
- ドローンを日常に導入している
- ボタンとスティックが付いたコントローラーではなく，カメラで直接飛んで欲しい場所を指定している
- 完全自動じゃなくて半自動  

## このアイディアの悪いところ  
- MITの研究(2014)とほぼ被ってしまっている
- 動的な被写体は撮影出来ない  
- 平面ではないところでは撮影できない(ARの場合)
- キャリブレーション方法が難しい


## References  
### Computational Rim Illumination with Aerial Robots(2014)  
URL:   
動画1: https://www.youtube.com/watch?v=fhob-WgAfQo  
動画2: https://www.youtube.com/watch?v=2R6AEDONbk8&t=1s  
#### 定義  
ダイナミックな被写体を撮影するため，(リム)ドローンをつかった照明とカメラの協調による新しい照明制御システム  

#### 背景と問題  
プロカメラマンは凄い設備を使って被写体を撮影する．でも，被写体が動いていると姿勢や動きによって照明を再配置しなければならないという大変手間な作業が必要である．  
対象: プロカメラマン  

#### 提案手法   
- ドローンを用いたすごい自動化照明というアプローチ
- 撮影するカメラの視点からのリム計算とドローンの被写体の追跡を組み合わせた制御アプローチ  

#### 実装方法  
ドローン: Parrot 2010; Bristeau et al. 2011   
航空学とかからも引っ張ってきたすごいアルゴリズム  
いい感じのドローンの制御方法もあるらしい  

#### 議論  
ドローンが写り込んでいたら話にならない気がする  

### ドローンが照らす、まるで異世界の砂漠  
URL: https://wired.jp/2017/01/15/drone-lighting-brings-deserts/  
