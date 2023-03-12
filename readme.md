- [探索 ReactNative](#探索-reactnative)
- [Question](#question)
    - [使用 pnpm 安装后无法启动](#使用-pnpm-安装后无法启动)

# 探索 ReactNative

# Question

### 使用 pnpm 安装后无法启动

具体问题是 RN 项目无法使用 symlinks [issure facebook/metro#1](https://github.com/facebook/metro/issues/1)

1. 使用 pnpm 时关闭 symlinks 配置， 需要 `.npmrc` 文件添加 `node-linker=hoisted`。[具体配置说明参考 pnpm 官网](https://pnpm.js.org/en/pnpmfile#node-linker)
2. 放弃 pnpm，改用 yarn/npm 安装依赖
