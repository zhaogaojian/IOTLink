该应用完全免费
# 界面整体
<img width="1920" height="1215" alt="image" src="https://github.com/user-attachments/assets/f81b225f-614b-42ef-bc36-72856f237fab" />
核心功能
# 发布主题
<img width="970" height="1090" alt="image" src="https://github.com/user-attachments/assets/0aad9bcb-1fb3-4d5f-a0f6-1ffde67f4c39" />

树形主题分组，支持文件夹与主题节点，便于管理大量 Topic。
每个主题可配置 QoS、Retain、编码方式（如 UTF-8 文本 / Hex）。
多页签编辑：Payload、Markdown 备注、发布前 JavaScript 预处理（动态改写负载）。
代码编辑器支持语法高亮、JSON 格式化等，提升编辑效率。
随发订阅：可按主题为「发布成功后自动向 Broker 订阅」单独配置过滤器；随发过滤可与订阅侧消息过滤分区同步，避免误覆盖用户自定义条件。
支持主题列表的打开 / 保存（JSON），便于备份与共享。
# 订阅主题
<img width="955" height="1085" alt="image" src="https://github.com/user-attachments/assets/ab3aac72-31ab-4a1b-9cac-42690ddd3044" />

多主题订阅列表，支持 + / # 通配符。
消息表格实时展示时间、主题、QoS、负载预览；可查看详情与 JSON 格式化。
多条消息过滤规则（主题 / 内容 / 全局 × 包含或不包含），并与发布侧随发过滤分区协同。
支持禁用 / 启用订阅项、导出等常用操作。
流式转换
<img width="955" height="1095" alt="image" src="https://github.com/user-attachments/assets/141f111c-3e8d-48a0-b4f4-6437b7b79eb7" />

多条转换规则：源主题监听 → JS 脚本变换 → 发布到目标主题。
规则可单独启用 / 禁用，带运行日志与简单统计，便于排查脚本问题。
提供测试区，便于在上线前验证脚本输出。
# 实时看板
<img width="964" height="1095" alt="image" src="https://github.com/user-attachments/assets/6f082019-4333-4dc2-bec0-d2adf283bf14" />

可配置 多行多列监视格，每格独立订阅主题（支持通配符）。
自动解析 JSON 对象 / 数组 或 多行「键=值」 文本，以表格形式展示键值，适合遥测、状态类 Topic 的 实时监视。
布局与格子配置可随窗口变化尽量 铺满停靠区域，减少无效留白。
# 方案管理（Project）
<img width="975" height="1090" alt="image" src="https://github.com/user-attachments/assets/815f6f78-4afc-40ee-8d8b-c90247f7dac6" />

# 系统脚本
<img width="950" height="1085" alt="image" src="https://github.com/user-attachments/assets/111e0561-c122-4dda-b910-55f857ac5982" />

# 任务管理
<img width="955" height="1084" alt="image" src="https://github.com/user-attachments/assets/580da077-f9a5-4179-ba5e-ac363deb0dad" />


以目录为单位管理 工程方案，集中保存发布树、订阅状态、流式规则及连接配置等，便于按项目或现场切换环境。
# 界面与使用体验

各功能置于 可停靠、可叠标签的 Dock 面板，便于双屏或大窗口并排调试。
主窗口 不设空白中央区，左右工作区可更好利用横向空间。
工具栏快速连接、多连接配置（Profile）等，适合多 Broker 切换。
# 适用场景
物联网设备与网关的 MQTT 联调、抓包与消息核对。
运维人员临时订阅生产 / 测试 Broker 做健康检查。
需在客户端侧做 轻量主题映射、字段改写 的演示或中转。
需要在单屏内 同时看多个 Topic 的键值状态 的监控场景。
# 系统与依赖说明
面向 Windows 桌面（具体最低版本以你实际测试为准，建议写明 Windows 10 及以上）。
基于 Qt 与 Qt MQTT 构建；发布包通常附带所需 Qt 运行库（以你实际打包方式为准）。
需自行准备可访问的 MQTT Broker（如 Mosquitto、EMQX 等）。




