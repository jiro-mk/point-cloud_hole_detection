# point-cloud_hole_detection


点群データ（平面プレート）から凹みの検出、体積の計算を行う

◆用途
・表面形状の外観検査

→ 写真では判別できない凹みや傷などを検出（暗い場所でも検出可）

→ 大きさ、体積を計算可能

![image](https://user-images.githubusercontent.com/93971055/221352463-7e3216af-38c0-4bb3-88ba-a7aef296dc5d.png)



# 処理の概要

・RANSACを用いて凹み部分を検出

・HDBSCANによるクラスタリングによって位置と個数を特定する

・プレートの体積を計算




# DEMO

検出する平面プレート

![image](https://user-images.githubusercontent.com/93971055/221352569-cd4bb9c5-5434-46a2-a1e9-2fd59a2616ef.png)

検出結果

![image](https://user-images.githubusercontent.com/93971055/221352608-0385494c-a62e-480f-87c0-7f9980a7e2ac.png)

```bash
clack num : 10

```


# Requirement

open3d

hdbscan

k3d

pyransac


