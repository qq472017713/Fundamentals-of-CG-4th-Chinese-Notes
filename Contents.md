科研(炼丹?) 做得比较迷茫, 回顾下学 CG 的初心

其实有其他大佬们([https://www.zhihu.com/column/c_1299028644052824064](https://www.zhihu.com/column/c_1299028644052824064)) 也在翻译这本书, 但自己还是给自己立个 Flag, 看自己单干能做多少吧

本人才疏学浅, 有什么 BUG 欢迎指正

---

1 介绍 (Introduction) 1

1.1 图形学不同领域 (Graphics Areas) . . . . . . . . . . . . . . . . . . . . . . . . . . 2

1.2 图形学主要应用 (Major Applications) . . . . . . . . . . . . . . . . . . . . . . . . 3

1.3 图形 APIs (Graphics APIs) . . . . . . . . . . . . . . . . . . . . . . . . . . 4

1.4 图形学管线 (Graphics Pipeline) . . . . . . . . . . . . . . . . . . . . . . . . . 4

1.5 数值问题( Numerical Issues) . . . . . . . . . . . . . . . . . . . . . . . . . 5

1.6 效率 (Efﬁciency) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7

1.7 图形程序的设计与编程 (Designing and Coding Graphics Programs) . . . . . . . . . . . . 8

2 各式各样的数学 (Miscellaneous Math) 13

2.1 集合与映射 (Sets and Mappings) . . . . . . . . . . . . . . . . . . . . . . . . 13

2.2 二次方程求解 (Solving Quadratic Equations) . . . . . . . . . . . . . . . . . . . 17

2.3 三角几何 (Trigonometry) . . . . . . . . . . . . . . . . . . . . . . . . . . . 18

2.4 向量 (Vectors) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 21

2.5 曲线和表面 (Curves and Surfaces) . . . . . . . . . . . . . . . . . . . . . . . 30

2.6 线性插值 (Linear Interpolation) . . . . . . . . . . . . . . . . . . . . . . . 44

2.7 三角形 (Triangles) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 44

3 栅格图像 (Raster Images)  53

3.1 栅格设备 (Raster Devices) . . . . . . . . . . . . . . . . . . . . . . . . . . 54

3.2 图像, 像素与几何 (Images, Pixels, and Geometry) . . . . . . . . . . . . . . . . . . 59

3.3 RGB 色彩 (RGB Color) . . . . . . . . . . . . . . . . . . . . . . . . . . . . 64

3.4 透明度混合 (Alpha Compositing) . . . . . . . . . . . . . . . . . . . . . . . . 65

4 光线追踪 (Ray Tracing) 69

4.1 基础光线追踪算法 (The Basic Ray-Tracing Algorithm) . . . . . . . . . . . . . . . . 70

4.2 透视 (Perspective) . . . . . . . . . . . . . . . . . . . . . . . . . . . . 71

4.3 计算可见光线 (Computing Viewing Rays) . . . . . . . . . . . . . . . . . . . . 73

4.4 光线-物体相交测试 (Ray-Object Intersection) . . . . . . . . . . . . . . . . . . . . . 76

4.5 着色(Shading) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 81

4.6 一个光线追踪程序 (A Ray-Tracing Program) . . . . . . . . . . . . . . . . . . . . . 84

4.7 阴影 (Shadows) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 86

4.8 理想的镜面(高光)反射 (Ideal Specular Reﬂection) . . . . . . . . . . . . . . . . . . . . . 87

4.9 历史进程(Historical Notes) . . . . . . . . . . . . . . . . . . . . . . . . . 87

5 线性代数 (Linear Algebra) 89

5.1 行列式(Determinants) . . . . . . . . . . . . . . . . . . . . . . . . . . . 89

5.2 矩阵 (Matrices) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 91

5.3 与行列式, 矩阵相关的计算 (Computing with Matrices and Determinants) . . . . . . . . . . . 96

5.4 特征值与矩阵的对角化 (Eigenvalues and Matrix Diagonalization) . . . . . . . . . . . . . 101

6 变换矩阵 (Transformation Matrices) 109

6.1 2D 线性变换 (2D Linear Transformations) . . . . . . . . . . . . . . . . . . . . 109

6.2 3D 线性变换 (3D Linear Transformations) . . . . . . . . . . . . . . . . . . . . 123

6.3 平移与仿射变换 (Translation and Afﬁne Transformations) . . . . . . . . . . . . . 128

6.4 变换矩阵的逆 (Inverses of Transformation Matrices) . . . . . . . . . . . . . . . 132

6.5 坐标变换 (Coordinate Transformations) . . . . . . . . . . . . . . . . . . . 133

7 视图 Viewing 139

7.1 视图变换 (Viewing Transformations) . . . . . . . . . . . . . . . . . . . . . 140

7.2 投影变换 (Projective Transformations) . . . . . . . . . . . . . . . . . . . . 146

7.3 透视投影 (Perspective Projection) . . . . . . . . . . . . . . . . . . . . . . 149

7.4 透视变换的一些属性 (Some Properties of the Perspective Transform) . . . . . . . . . . 153

7.5 视野范围 (Field-of-View) . . . . . . . . . . . . . . . . . . . . . . . . . . . 154

8 图形学管线 (The Graphics Pipeline) 159

8.1 光栅化 (Rasterization) . . . . . . . . . . . . . . . . . . . . . . . . . . . 160

8.2 那些光栅化之前和之后所做的事情 (Operations Before and After Rasterization) . . . . . . . 171

8.3 简单抗锯齿 (Simple Antialiasing) . . . . . . . . . . . . . . . . . . . . . . . . 177

8.4 裁剪图元Culling Primitives for Efﬁciency . . . . . . . . . . . . . . . . . 179

9 信号处理 (Signal Processing) 183

9.1 数字音频: 在 1D 空间的采样 (Digital Audio: Sampling in 1D) . . . . . . . . . . . . . . . . . . 184

9.2 卷积 (Convolution) . . . . . . . . . . . . . . . . . . . . . . . . . . . . 187

9.3 卷积滤波器 (Convolution Filters) . . . . . . . . . . . . . . . . . . . . . . . . 201

9.4 对图像的信号处理 (Signal Processing for Images) . . . . . . . . . . . . . . . . . . . 208

9.5 采样理论 (Sampling Theory) . . . . . . . . . . . . . . . . . . . . . . . . . 217

10 表面着色 (Surface Shading) 233

10.1 漫反射着色 (Diffuse Shading) . . . . . . . . . . . . . . . . . . . . . . . . . 233

10.2 Phong 着色 (Phong Shading) . . . . . . . . . . . . . . . . . . . . . . . . . . 236

10.3 艺术风格 着色 (Artistic Shading) . . . . . . . . . . . . . . . . . . . . . . . . . 239

11 纹理贴图 (Texture Mapping) 243

11.1 纹理值查询 (Looking Up Texture Values) . . . . . . . . . . . . . . . . . . . 244

11.2 纹理坐标函数 (Texture Coordinate Functions). . . . . . . . . . . . . . . . . . 246

11.3 带抗锯齿的纹理查询 (Antialiasing Texture Lookups) . . . . . . . . . . . . . . . . . . 260

11.4 纹理贴图的应用 (Applications of Texture Mapping) . . . . . . . . . . . . . . . . 267

11.5 程序化的 3D 纹理 (Procedural 3D Textures) . . . . . . . . . . . . . . . . . . . . . . 273

12 图形学中的数据结构 (Data Structures for Graphics) 281

12.1 三角网格 (Triangle Meshes) . . . . . . . . . . . . . . . . . . . . . . . . . 282

12.2 场景图 (Scene Graphs) . . . . . . . . . . . . . . . . . . . . . . . . . . . 295

12.3 空间数据结构 (Spatial Data Structures) . . . . . . . . . . . . . . . . . . . . . . 297

12.4 BSP 树的可见度 (BSP Trees for Visibility) . . . . . . . . . . . . . . . . . . . . . 309

12.5 平铺多维数组 (Tiling Multidimensional Arrays) . . . . . . . . . . . . . . . . . 317

13 更多的光线追踪 (More Ray Tracing) 323

13.1 透明度和折射 (Transparency and Refraction) . . . . . . . . . . . . . . . . . . . 324

13.2 实例化 (Instancing) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 327

13.3 CSG (Constructive Solid Geometry) . . . . . . . . . . . . . . . . . . . 328

13.4 分布式光线追踪 (Distribution Ray Tracing) . . . . . . . . . . . . . . . . . . . . . 329

14 采样 (Sampling) 337

14.1 积分 (Integration) . . . . . . . . . . . . . . . . . . . . . . . . . . . . 337

14.2 连续概率 (Continuous Probability) . . . . . . . . . . . . . . . . . . . . . . 342

14.3 蒙特卡洛积分Monte Carlo Integration . . . . . . . . . . . . . . . . . . . . . 346

14.4 随机点的选择 (Choosing Random Points) . . . . . . . . . . . . . . . . . . . . . 349

15 曲线 (Curves) 359

15.1 曲线 (Curves) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 359

15.2 曲线属性 (Curve Properties) . . . . . . . . . . . . . . . . . . . . . . . . . 365

15.3 多项式分段 (Polynomial Pieces) . . . . . . . . . . . . . . . . . . . . . . . . 368

15.4 分段汇总 (Putting Pieces Together) . . . . . . . . . . . . . . . . . . . . . . 375

15.5 三次曲线 (Cubics) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 378

15.6 近似曲线 (Approximating Curves) . . . . . . . . . . . . . . . . . . . . . . 385

15.7 总结 (Summary) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 402

16 计算机动画 (Computer Animation) 405

16.1 动画原则 (Principles of Animation) . . . . . . . . . . . . . . . . . . . . . 406

16.2 关键帧 (Keyframing) . . . . . . . . . . . . . . . . . . . . . . . . . . . . 410

16.3 变形 (Deformations) . . . . . . . . . . . . . . . . . . . . . . . . . . . 418

16.4 角色动画 (Character Animation). . . . . . . . . . . . . . . . . . . . . . . 419

16.5 基于物理的动画 (Physics-Based Animation) . . . . . . . . . . . . . . . . . . . . 426

16.6 程序化技术 (Procedural Techniques) . . . . . . . . . . . . . . . . . . . . . . 428

16.7 对象编组 (Groups of Objects) . . . . . . . . . . . . . . . . . . . . . . . . 431

17 图形化硬件 (Using Graphics Hardware) 437

17.1 硬件概览 (Hardware Overview) . . . . . . . . . . . . . . . . . . . . . . . 437

17.2 什么是图形学硬件 (What Is Graphics Hardware) . . . . . . . . . . . . . . . . . . . 437

17.3 异构多线程 (Heterogeneous Multiprocessing) . . . . . . . . . . . . . . . . . 439

17.4 图形硬件编程 (Graphics Hardware Programming: Buffers, State, and Shaders) . 441 

17.5 状态机 (State Machine) . . . . . . . . . . . . . . . . . . . . . . . . . . . 443

17.6 基础的 OpenGL 应用结构 (Basic OpenGL Application Layout) . . . . . . . . . . . . . . . 444

17.7 几何 (Geometry) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 445

17.8 Shaders 初印象 (A First Look at Shaders) . . . . . . . . . . . . . . . . . . . . . 447

17.9 顶点缓存对象 (Vertex Buffer Objects) . . . . . . . . . . . . . . . . . . . . . . . 450

17.10 顶点数组对象 (Vertex Array Objects) . . . . . . . . . . . . . . . . . . . . . . . 452

17.11 变换矩阵 (Transformation Matrices) . . . . . . . . . . . . . . . . . . . . . 455

17.12 逐顶点着色 (Shading with Per-Vertex Attributes) . . . . . . . . . . . . . . . 457

17.13 逐片段着色 (Shading in the Fragment Processor) . . . . . . . . . . . . . . . . 461

17.14 网络和实例化 (Meshes and Instancing) . . . . . . . . . . . . . . . . . . . . . . 467

17.15 纹理对象 (Texture Objects) . . . . . . . . . . . . . . . . . . . . . . . . . . 469

17.16 面向对象的图形学硬件编程 (Object-Oriented Design for Graphics Hardware Programming) . 475 

17.17 下一步学习? (Continued Learning) . . . . . . . . . . . . . . . . . . . . . . . 476

18 光照 (Light) 479

18.1 辐射 (Radiometry) . . . . . . . . . . . . . . . . . . . . . . . . . . . . 479

18.2 光线传输方程 (Transport Equation) . . . . . . . . . . . . . . . . . . . . . . . . 488

18.3 光度学 (Photometry) . . . . . . . . . . . . . . . . . . . . . . . . . . . . 489

19 颜色 (Color) 493

19.1 色度学 (Colorimetry) . . . . . . . . . . . . . . . . . . . . . . . . . . . . 495

19.2 颜色空间 (Color Spaces) . . . . . . . . . . . . . . . . . . . . . . . . . . . 504

19.3 色彩适应 (Chromatic Adaptation) . . . . . . . . . . . . . . . . . . . . . . 510

19.4 色彩外观 (Color Appearance) . . . . . . . . . . . . . . . . . . . . . . . . 514

20 视觉感知 (Visual Perception) 515

20.1 视觉科学 (Vision Science) . . . . . . . . . . . . . . . . . . . . . . . . . . 516

20.2 可视化敏感度 (Visual Sensitivity) . . . . . . . . . . . . . . . . . . . . . . . . . 517

20.3 空间视觉 (Spatial Vision) . . . . . . . . . . . . . . . . . . . . . . . . . . . 534

20.4 物体, 位置和事件 (Objects, Locations, and Events) . . . . . . . . . . . . . . . . . . 547

20.5 图像感知 (Picture Perception) . . . . . . . . . . . . . . . . . . . . . . . . 556

21 色调重构 (Tone Reproduction) 559

21.1 分类 (Classiﬁcation) . . . . . . . . . . . . . . . . . . . . . . . . . . . 562

21.2 动态范围 (Dynamic Range) . . . . . . . . . . . . . . . . . . . . . . . . . . 563

21.3 颜色 (Color) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 565

21.4 成像 (Image Formation) . . . . . . . . . . . . . . . . . . . . . . . . . 567

21.5 基于频率的 Operator (Frequency-Based Operators) . . . . . . . . . . . . . . . . . . . 567

21.6 梯度域 Operators (Gradient-Domain Operators) . . . . . . . . . . . . . . . . . . . 569

21.7 空间 Operators (Spatial Operators) . . . . . . . . . . . . . . . . . . . . . . . . . 570

21.8 除法 (Division) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 572

21.9 Sigmoids 函数 (Sigmoids) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 573

21.10 其它方法 (Other Approaches) . . . . . . . . . . . . . . . . . . . . . . . . 578

21.11 夜间色调映射 (Night Tone mapping) . . . . . . . . . . . . . . . . . . . . . . . 581

21.12 讨论 Discussion . . . . . . . . . . . . . . . . . . . . . . . . . . . . 582

22 隐式建模 (Implicit Modeling) 585

22.1 隐式函数, 骨架化图元以及 Blending 方法 (Implicit Functions, Skeletal Primitives, and Summation Blending) . . . . . . . . . . . .  . . . . . . 586

22.2 渲染 (Rendering) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 594

22.3 空间划分 (Space Partitioning) . . . . . . . . . . . . . . . . . . . . . . . . 595

22.4 Blending 的更多方法 (More on Blending) . . . . . . . . . . . . . . . . . . . . . . . . 601

22.5 CSG 建模 (Constructive Solid Geometry) . . . . . . . . . . . . . . . . . . 602

22.6 Warping . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 604

22.7 Precise Contact Modeling . . . . . . . . . . . . . . . . . . . . 606

22.8 The BlobTree . . . . . . . . . . . . . . . . . . . . . . . . . . . 608

22.9 交互式的隐式建模系统 (Interactive Implicit Modeling Systems) . . . . . . . . . . . . . . 610

23 全局光照 (Global Illumination) 613

23.1 对于兰伯特场景的粒子追踪 (Particle Tracing for Lambertian Scenes). . . . . . . . . . . . . 614

23.2 路径追踪 (Path Tracing) . . . . . . . . . . . . . . . . . . . . . . . . . . . 617

23.3 精确的直接光照 (Accurate Direct Lighting) . . . . . . . . . . . . . . . . . . . . . 619

24 反射模型 (Reﬂection Models) 627

24.1 真实世界的材质 (Real-World Materials) . . . . . . . . . . . . . . . . . . . . . . . 627

24.2 实现反射模型 (Implementing Reﬂection Models) . . . . . . . . . . . . . . . . . 629

24.3 镜面反射模型 (Specular Reﬂection Models) . . . . . . . . . . . . . . . . . . . 631

24.4 Smooth-Layered Model . . . . . . . . . . . . . . . . . . . . . 632

24.5 Rough-Layered Model . . . . . . . . . . . . . . . . . . . . . . 635

25 CG 在游戏中的应用 (Computer Graphics in Games) 643

25.1 平台 (Platforms) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 643

25.2 受限的资源 (Limited Resources) . . . . . . . . . . . . . . . . . . . . . . . . 646

25.3 优化技术 (Optimization Techniques) . . . . . . . . . . . . . . . . . . . . . 649

25.4 游戏类型 (Game Types) . . . . . . . . . . . . . . . . . . . . . . . . . . . 650

25.5 游戏开发流程 (The Game Production Process) . . . . . . . . . . . . . . . . . . 653

26 可视化 (Visualization) 665

26.1 背景 (Background) . . . . . . . . . . . . . . . . . . . . . . . . . . . . 667

26.2 数据类型 (Data Types) . . . . . . . . . . . . . . . . . . . . . . . . . . . . 668

26.3 以人为中心的设计 (Human-Centered Design Process) . . . . . . . . . . . . . . . . 670

26.4 可视化编码原则 (Visual Encoding Principles) . . . . . . . . . . . . . . . . . . . . 672

26.5 交互原则 (Interaction Principles) . . . . . . . . . . . . . . . . . . . . . . . 680

26.6 复合及邻接视图 (Composite and Adjacent Views) . . . . . . . . . . . . . . . . . 681

26.7 数据降维 (Data Reduction) . . . . . . . . . . . . . . . . . . . . . . . . . . 687

26.8 示例 (Examples) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 692