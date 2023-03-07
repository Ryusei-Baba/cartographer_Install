# cortographer使い方例
```
roslaunch cartographer_ros demo_backpack_2d.launch bag_filename:=${HOME}/Downloads/cartographer_paper_deutsches_museum.bag
```
### [Cortographer ROS](https://google-cartographer-ros.readthedocs.io/en/latest/demos.html)
---
# cartographerインストール
### [Cartographer をラズパイ4 単体で使う](https://qiita.com/devemin/items/1723058cf3bac85aaa0b)
1. ワークスペースを作成
```
mkdir -p cartographer_ws/src
```
2. cartographer_wsに移動
```
cd cartographer_ws/
```

3. error処理

- 3.1 pip listでjinja2<3.1か確認(2022年8月現在の場合)   
  - jinja2>3.1ならアンインストールして低いバージョンをインストール   
  (2022年8月現在の場合．2023年などでは違うバージョンの可能性あり)
```
pip list
```
```
pip uninstall jinja2
pip install jinja2==3.0.3
pip list
```
- 3.2 absei

### [Google CartographerとAbseil](https://kim-xps12.github.io/b-sky-lab/technology/2020/11/28/cartographerAbseil.html)
