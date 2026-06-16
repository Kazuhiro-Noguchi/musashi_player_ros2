# Musashi Player ROS2

[English](README.en.md)

ROS 2 Jazzy を用いた MUSASHI ロボットプラットフォームです。

本プロジェクトは、RoboCup Middle Size League (MSL) を想定したロボットソフトウェア基盤として開発されています。

## 特徴

* ROS 2 Jazzy
* Gazebo Harmonic シミュレーション
* Docker + Dev Container 対応
* EPOS2 を用いた実機制御
* RoboCup MSL 向けの拡張可能なアーキテクチャ
* シミュレーションから実機への移行を考慮した設計

## ディレクトリ構成

```text
musashi_player_ros2/
├── .devcontainer/
├── docker-compose.yml
├── src/
│   ├── behavior/
│   ├── bringup/
│   ├── communication/
│   ├── hardware/
│   ├── simulation/
│   └── vision/
├── LICENSE
└── README.md
```

### behavior

戦略・行動決定関連。

### bringup

Launch ファイルおよびシステム起動設定。

### communication

CoachBoxなど通信関連。

### hardware

実機デバイスとのインタフェース。

### simulation

Gazebo シミュレーション関連。

### vision

画像取得および認識処理。

## 開発環境

* Ubuntu 24.04
* Docker
* VS Code
* Dev Containers
* ROS 2 Jazzy
* Gazebo Harmonic

## セットアップ

### 1. リポジトリの取得

```bash
git clone <repository-url>
cd musashi_player_ros2
```

### 2. Dev Container を起動

VS Code でプロジェクトを開き、

```
Dev Containers: Reopen in Container
```

を実行してください。

### 3. ビルド

```bash
source /opt/ros/jazzy/setup.bash

colcon build --symlink-install

source install/setup.bash
```

## ライセンス

本プロジェクトのライセンスは LICENSE を参照してください。
