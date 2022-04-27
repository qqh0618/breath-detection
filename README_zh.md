# 基于视频的脉搏及心率检测
2022/4/27 基本调试

### 环境安装
1. 方法一 `pip install -r requirments`
2. 方法二 `conda env create -f enviroment.yaml`

### 运行
运行格式 `python breath_detector.py args1 args2 args3 `
- 注 `args1为视频名称, args2 视频后缀, args3为是否需要处理视频, 0为需要, 1为不需要，已经有json文件的话可以为1,以参数0运行时会生成json文件.  `

运行实例 `python brerath_detector.py Eugene MOV 0`

### 程序执行流程
播放选定的视频，显示胸部、面部和额头。他们将被视为脉搏和呼吸。动态图显示呼吸阶段，视频窗口显示当前脉搏和呼吸频率。播放结束时，会出现呼吸统计。您可以随时按Q键完成工作。