# 项目文档索引

## 文档结构

```
.monkeycode/docs/
├── INDEX.md              # 文档索引（本文件）
├── ARCHITECTURE.md       # 系统架构文档
└── 核心概念/
    └── 核心概念.md       # 核心概念详解
```

## 文档列表

### ARCHITECTURE.md

系统架构文档，包含：
- 项目概述与核心价值
- 系统架构图
- API 端点说明
- 目录结构
- 核心模块详解（handler、openai-handler、converter 等）
- 配置系统
- 核心技术特性
- API 兼容性矩阵
- 日志系统
- 启动与部署
- 注意事项

### 核心概念/核心概念.md

深入讲解项目中的核心概念：
- 协议转换（Anthropic ↔ Cursor）
- 身份保护（三层防御机制）
- 截断检测与续写
- 历史压缩
- 视觉处理
- 代理支持
- Token 估算

## 源码模块对应

| 文件 | 功能 |
|------|------|
| `src/handler.ts` | Anthropic Messages API 处理器 |
| `src/openai-handler.ts` | OpenAI 兼容处理器 |
| `src/converter.ts` | 核心协议转换器 |
| `src/cursor-client.ts` | Cursor API 客户端 |
| `src/tool-fixer.ts` | 工具参数修复 |
| `src/vision.ts` | 视觉处理 |
| `src/logger.ts` | 日志系统 |
| `src/log-viewer.ts` | 日志查看器 API |
| `src/config.ts` | 配置管理 |
| `src/tokenizer.ts` | Token 估算 |
| `src/streaming-text.ts` | 流式文本处理 |
| `src/proxy-agent.ts` | 代理支持 |
| `src/constants.ts` | 常量定义 |
| `src/types.ts` | 类型定义 |
