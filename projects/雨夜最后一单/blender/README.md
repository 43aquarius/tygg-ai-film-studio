# blender/ · 阶段 4：预演工程（待产出）

本目录承接资产图提示词包（阶段 3），按以下顺序产出：

## 制作顺序

1. **静态场景搭建**（中性色代理，无需贴图）
   - 人物代理按 `canon/人物设定.md` 参数：CHR_001（H1.78 / 胶囊1.30 / 头心1.62 / 头径0.22 / #5B7A8C）、CHR_002（H1.72 / 胶囊1.25 / 头心1.57 / 头径0.21 / #D98E4A）
   - 楼道布景（LOC_003）一次搭建，覆盖 SH_040 / SH_070 / SH_080 同机位复用
2. **角色路径 + 相机动画粗排**（13 镜逐镜）
   - 可见手部仅 SH_060（右手简化 IK 递袋）
3. **逐镜 playblast 导出**（Workbench 着色器，960×540，约 3.1s/帧 @ low 档预算）

## 环境备注

- 预演验证环境：Blender 5.2.2 headless（`--background --python` 通道）+ lavapipe Vulkan（Workbench）
- 已验证能力：Workbench/lavapipe 渲染、Cycles CPU、4 骨骼链分层 Action、Follow Path 约束
- 注：沙盒制作环境在阶段 4 开始前被重置（Blender 安装与验证记录一并丢失），恢复制作时需重新部署上述环境。
