# FuckClassroom AI 总结插件

FuckClassroom 的独立 AI 总结插件，插件 ID 为 `ai_summary`。

## 功能

- 将课程转写与 PPT OCR 文本整理为结构化学习笔记
- 独立 Worker 进程执行 AI 请求
- 向 OCR 插件提供可选视觉 OCR 能力
- 通过宿主稳定 RPC 桥接 `ai_summary.ocr.image`，不与 OCR 源码耦合

## 依赖

- FuckClassroom: `>=0.1,<0.3`
- Plugin API: `1`
- Required plugin: `processing`
- 无额外 Python 第三方依赖

OCR 不是本插件的硬依赖；即使 OCR 插件未安装，课程总结功能也可正常使用。

## 开发

开发分支为 `plugin-management`。合并到 `main` 后，CI 成功会自动发布 Registry v1 beta Release。
