# Vue 3 + Vite
# AI助手对话组件

## 项目概述
这是一个基于 Vue 3 的 AI 对话单页应用，实现了用户与 AI 助手的实时交互功能。用户可输入问题并获取 AI 模型的回复，界面包含对话历史展示、消息输入及提交功能。

## 使用的模型/API方式
- **API服务地址**：`https://ark.cn-beijing.volces.com/api/v3/chat/completions`
- **使用模型**：`doubao-1-5-lite-32k-250115`
- **认证方式**：采用Bearer Token进行API身份验证（代码中已包含示例令牌）

## 如何运行/测试

### 前置条件
- 安装Node.js 14.0.0及以上版本
- 具备有效的网络连接

### 运行步骤
1. 将组件代码集成到您的Vue3项目中
2. （可选）替换API请求中的Authorization令牌为您自己的有效令牌：
   ```javascript
   'Authorization': 'Bearer 您的令牌'
   ```
3. 安装项目依赖：
   ```bash
   npm install
   # 或
   yarn install
   ```
4. 启动开发服务器：
   ```bash
   npm run dev
   # 或
   yarn dev
   ```
5. 在浏览器中访问项目地址（`http://localhost:5173`）即可使用

## 开发说明

### 借助ChatGPT/搜索完成的部分
- API请求的参数配置和格式参考了豆包API官方文档
- 错误处理机制和异步操作流程设计借助了 ChatGPT 的思路建议
- 滚动到底部的逻辑实现参考了Vue3滚动处理的最佳实践

### 功能特点
- 支持用户与AI的实时对话交互
- 支持Enter键快捷发送消息
- 自动滚动到最新消息位置# ai_project
