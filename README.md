# cartographerインストール
1. cart.zipをダウンロードし適当な場所に展開
2. ワークスペースを作成
```
mkdir -p cartographer_ws/src
```
3. 展開したファイル(cartographer, cartographer_ros)をsrcに移動させる．   
4. cartographer_wsに移動
```
cd cartographer_ws/
```
5. catkin buildでビルド．エラーが出たら，6以降の依存関係を確認する．
```
catkin build
```
6. pip listでjinja2<3.1か確認(2022年8月現在の場合)   
```
pip list
```
7. jinja2>3.1ならアンインストールして低いバージョンをインストール   
  (2022年8月現在の場合．2023年などでは違うバージョンの可能性あり)
```
pip uninstall jinja2
pip install jinja2==3.03
pip list
```
8. catkin buildでビルド
```
catkin build
```
