# ego-videoframe
> Simplified open-source offline workspace of EgoHome PC for egocentric hand-object interaction annotation & visual review.

## 📌 Overview
`ego-videoframe` is a local GUI tool for embodied AI researchers and students.
It focuses on **reviewing and manually refining pre-computed inference results** from egocentric videos.

✅ All data stays locally. No video / annotation data upload to any server.
✅ Load external HaMeR / MANO hand poses, object bounding boxes, segmentation masks and contact labels.
✅ Time-axis alignment check, skeleton editing, mask brush, hand-object contact marking, atomic action segmentation.
✅ Native exporter for LeRobot v2.0 dataset format.

⚠️ **Important boundary**
This open-source edition **DOES NOT contain built-in AI inference, model download, cloud collaboration, task queue or MuJoCo simulation modules**.
You need to run HaMeR, SAM, detection models on your own environment and import the generated JSON results into this tool.
Advanced features are available in the closed-source **EgoHome PC-Pro**.

## 🧩 Typical Workflow
1. Record egocentric video on your mobile device
2. Run hand/object models (HaMeR / SAM / OWLv2) externally, get JSON outputs
3. Load video + inference results into ego-videoframe
4. Visually check, manually correct skeletons, masks, contact events and split atomic actions
5. Run simple rule-based quality check and export datasets

## 🤝 Contribution
Bug fixes, UI improvement, decoder compatibility and export format PRs are welcome.
Feature requests for built-in AI inference / cloud service will be directed to EgoHome PC-Pro.

## 📄 License
Apache License 2.0

---

# ego-videoframe 是 EgoHome PC 的简化开源单机工作台，面向具身智能方向科研人员与学生。

本软件为纯本地GUI工具，核心用于**复核、手工修正外部算法产出的 ego 第一人称推理结果**。
✅ 所有数据本地运行，视频和标注文件不上传云端
✅ 支持导入外部 HaMeR / MANO 手部姿态、物体框、遮罩、接触标注结果
✅ 时序轴对齐校验、骨架拖拽编辑、笔刷遮罩、手物接触标记、原子动作片段切分
✅ 原生支持导出 LeRobot v2.0 数据集格式

⚠️ **功能边界（必读）**
本开源版本**不内置AI推理、模型自动下载、云端小组协同、批量任务队列、MuJoCo仿真模块**。
你需要自己在外部环境运行 HaMeR、SAM、检测模型，生成 JSON 结果后导入本软件。
全套高级能力在闭源版本 **EgoHome PC-Pro** 提供。

## 🧩 使用流程
1. 手机录制第一人称视频
2. 外部独立运行手部/视觉模型（HaMeR / SAM / OWLv2），得到标注JSON
3. 在 ego-videoframe 加载视频与推理结果
4. 可视化复核，手动修正骨架、遮罩、接触事件，切分原子动作
5. 基础规则质检，导出数据集

## 🤝 贡献
欢迎提交 Bug 修复、UI优化、解码兼容、导出格式扩展类 PR。
内置AI推理、云端相关的功能需求，将引导至 EgoHome PC-Pro。

## 📄 开源协议
Apache License 2.0
