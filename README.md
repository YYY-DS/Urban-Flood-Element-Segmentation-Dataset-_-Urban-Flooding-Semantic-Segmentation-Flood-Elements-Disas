# 城市洪水要素分割数据集  | 城市洪涝 语义分割 洪水要素 灾害监测 灾后评估  城市洪涝场景下的多类别地物与洪水要素的像素级语义分割9158期

## 数据集概述

本数据集专注于**城市洪涝场景下的多类别地物与洪水要素的像素级语义分割**，服务于城市洪涝灾害监测、灾后评估及应急响应。数据涵盖22类城市地物与洪水相关目标，适配无人机航拍巡检、灾害范围提取及城市洪涝智能分析等应用。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/15df1a0bf71c416d8ed12fdb5fb9d045.png)

## 数据集核心信息

| 数据要素 | 详细说明 |
| :--- | :--- |
| **类别** | 共 **22** 类（详见下方列表） |
| **数量** | **5971** 张图像 |
| **格式** | 图像为 JPG/PNG（分辨率 **1080×1920**）；同时提供 **YOLO** 与 **VOC** 两种标注格式 |
| **数据划分** | 训练集 **4180** 张，验证集 **1195** 张，测试集 **596** 张 |
| **应用价值** | 1. **城市洪涝监测**：支撑城市洪水淹没范围、破坏区域的自动化提取。<br>2. **灾后评估**：量化建筑、道路、车辆等要素的受淹情况，辅助损失评估与重建规划。<br>3. **应急响应**：快速定位受淹区域与基础设施损毁情况，指导救援力量部署。<br>4. **算法研发**：为城市洪涝语义分割、多类别地物识别等视觉任务提供大规模训练与评测数据。 |


![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/93d77d645d314508a1acf2520d058b1f.png)

## 完整类别列表（共22类）

| 序号 | 英文名称 | 中文释义 | 图像数 | 标注数 |
|:---:|:---|:---|:---:|:---:|
| 1 | river_levee_level2 | 河流堤坝 | 1466 | 2186 |
| 2 | river_flood damaged area_level2 | 河流洪水破坏区域 | 1827 | 2491 |
| 3 | river_flood debris damaged area_level2 | 河流洪水残骸破坏区域 | 1172 | 1885 |
| 4 | river_dam_level2 | 河流大坝 | 504 | 18 |
| 5 | river_bridge-pier_level2 | 河流桥梁-桥墩 | 829 | 598 |
| 6 | city_building_level2 | 城市建筑 | 938 | 1460 |
| 7 | city_flood damaged area_level2 | 城市洪水破坏区域 | 3334 | 5260 |
| 8 | city_flood debris damaged area_level2 | 城市洪水残骸破坏区域 | 1094 | 1965 |
| 9 | city_car_level2 | 城市汽车 | 1021 | 1825 |
| 10 | city_landslide_level2 | 城市滑坡 | 426 | 19 |
| 11 | city_person_level2 | 城市人物 | 833 | 1077 |
| 12 | city_car traffic light_level2 | 城市汽车交通灯 | 613 | 277 |
| 13 | city_pedestrian traffic light_level2 | 城市行人交通灯 | 442 | 223 |
| 14 | city_traffic sign_level2 | 城市交通标志 | 446 | 396 |
| 15 | city_distance sign_level2 | 城市距离标志 | 413 | 280 |
| 16 | city_road_level2 | 城市道路 | 628 | 632 |
| 17 | common_telegraph pole_level2 | 通用电线杆 | 473 | 1197 |
| 18 | common_flood damaged area_level2 | 通用洪水破坏区域 | 1850 | 2392 |
| 19 | common_flood debris damaged area_level2 | 通用洪水残骸破坏区域 | 360 | 727 |
| 20 | common_street lamp_level2 | 通用路灯 | 417 | 942 |
| 21 | common_tree_level2 | 通用树木 | 458 | 1510 |
| 22 | common_underpass_level2 | 通用下穿通道 | 845 | 286 |


![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/75a1fc6683ad42a48dc02a92a2d34692.png)

## 数据三要素解析

**类别与目标覆盖**
*   数据集定义 **22** 类城市地物与洪水相关目标，覆盖 **洪水要素类**（洪水破坏区域、洪水残骸破坏区域）、**基础设施类**（建筑、道路、桥梁-桥墩、堤坝、大坝、下穿通道）、**交通设施类**（汽车、交通灯、交通标志、距离标志）、**自然要素类**（树木、滑坡）及 **市政设施类**（电线杆、路灯）。
*   类别设置覆盖了城市洪涝场景中的主要要素，具有较强的系统性。
*   类别命名后缀“_level2”表明这可能是一个多层级标注体系中的第二层级。

**数据规模与划分**
*   图像总量约 **5971** 张，按约 **70:20:10** 比例划分为训练集（4180张）、验证集（1195张）与测试集（596张），划分规范。
*   图像分辨率为 **1080×1920**，属高清竖版图像，适合航拍或移动端采集场景。
*   同时提供 **YOLO** 与 **VOC** 双格式标注，灵活适配不同检测与分割框架。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/b1c4e48fbb4241bf92be3a6d0c56101b.png)

**应用与扩展**
*   数据集可扩展用于 **多层级语义分割**（level1/level2联合分析）、**洪水淹没时序监测** 及 **灾后重建优先级评估**。
*   可结合 **地理信息系统（GIS）** 生成城市洪涝分布图，辅助应急指挥与城市规划。
*   数据可迁移至 **其他城市洪涝场景** 的分割任务，进行微调适配。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/659ae64bed1e4b1a803446cf34e51741.png)

## 知识普及：城市洪涝语义分割的技术要点

*   **类间相似性挑战**：洪水破坏区域与洪水残骸破坏区域在视觉上可能相近；城市建筑与淹没建筑需依赖上下文信息区分。
*   **多类别分割难度**：22类的细粒度分类对模型的特征提取能力要求极高，需采用深层骨干网络与多尺度特征融合。
*   **类别不平衡**：部分类别样本极少（如河流大坝仅18个标注、城市滑坡仅19个标注），训练时需采用类别加权损失或过采样策略。
*   **高分辨率处理**：1080×1920 的图像对显存要求较高，建议采用裁切或降采样策略。
*   **背景干扰**：城市环境复杂，阴影、反光、雨雾等可能影响分割效果，建议训练时加入相关数据增强。
*   **应用闭环**：分割结果可导入GIS系统，生成城市洪涝态势图与灾损报告，服务于应急决策。

## 快速开始（代码示例）

配置文件 `data.yaml` 示例：
```yaml
train: ./dataset/images/train
val: ./dataset/images/val
test: ./dataset/images/test
nc: 22
names: ['river_levee_level2', 'river_flood damaged area_level2', 
        'river_flood debris damaged area_level2', 'river_dam_level2', 
        'river_bridge-pier_level2', 'city_building_level2', 
        'city_flood damaged area_level2', 'city_flood debris damaged area_level2', 
        'city_car_level2', 'city_landslide_level2', 'city_person_level2', 
        'city_car traffic light_level2', 'city_pedestrian traffic light_level2', 
        'city_traffic sign_level2', 'city_distance sign_level2', 
        'city_road_level2', 'common_telegraph pole_level2', 
        'common_flood damaged area_level2', 'common_flood debris damaged area_level2', 
        'common_street lamp_level2', 'common_tree_level2', 'common_underpass_level2']
```

启动 YOLOv8 语义分割训练：
```python
from ultralytics import YOLO

model = YOLO('yolov8m-seg.pt')
model.train(
    data='data.yaml',
    epochs=100,
    imgsz=640,
    batch=8,
    device=0
)
```

## 标签
`城市洪涝` `语义分割` `洪水要素` `灾害监测` `灾后评估` `目标检测` `YOLO格式` `深度学习数据集` `计算机视觉`
