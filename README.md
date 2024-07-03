# ue5-boids-simulation
* Boidsアルゴリズムによる群衆シミュレーションサンプルになります。
  * Niagaraを用いて実装しており、シミュレーション計算はSimulationStageを使用、オブジェクトはパーティクルとして描画しています。

<img width=600 src="/ReadMeContents/01_boids3d.png"></img>

## バージョン
* UnrealEngine
  * 5.3.2

## 使い方

### シミュレーションの実装内容について
* <a href="/Content/Boids/NS_BoidsSimulation.uasset">Boids/NS_BoidsSimulation.uasset</a>にて実装してあります。

### レベルについて
  * <a href="/Content/Map/Boids.umap">Map/Boids.umap</a> をご覧ください。

### シミュレーションのパラメータ

<img width=320 src="/ReadMeContents/02_boids3d_parameters.png"></img>

| パラメータ | 概要 |
| - | - |
| AlignmentCoefficient | 適用時の重み係数: 整列 |
| AlignmentDistance | 適用する他の個体との半径: 整列 |
| CohesionCoefficient | 適用時の重み係数: 結合 |
| CohesionDistance | 適用する他の個体との半径: 結合 |
| N | Boids最大数 |
| SeparationCoefficient | 適用時の重み係数: 分離 |
| SeparationDistance | 適用する他の個体との半径: 分離 |
| SpaceScale | シミュレーション範囲 サイズ |
| WallAvoidanceCoefficient | 壁を避ける強さの重み |
