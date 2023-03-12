> 声明：此项目只用于演示和测试，请勿用于商业用途！
> 
> This project is for demonstration and testing purposes only. Please do not use it for commercial purposes!

# CustomGPT

基于ChatGPT API开发的纯前端应用

## 在线查看
https://www.customgpt.top/

## 功能特性

- 与chatGPT官网一致的问答功能
- 自定义API参数
- 自定义API baseUrl
- 保存配置参数
- 保存消息列表

## 使用方式
 1. [获取ApiKey](https://platform.openai.com/account/api-keys/)。
 2. 在右上角设置中修改API参数，支持配置文件保存和读取。
 3. 随时保存你的对话，比如保存[调教好的咒语](https://github.com/PlexPt/awesome-chatgpt-prompts-zh)，方便下次使用。

> 所有的配置和ApiKey均保存在本地，服务端不保存任何内容

## 已知问题

- Markdown渲染：文字动态变化时会造成页面闪烁
- logit_bias 配置
  - 不能正确解析中文tokenID
  - 按照[官方说明](https://help.openai.com/en/articles/5247780-using-logit-bias-to-define-token-probability)使用此参数不能达到预期效果
  - 数值较大时会造成输出异常或请求过慢的问题

## 开发

本项目使用 [Angular CLI](https://github.com/angular/angular-cli) 15.2.1 版本生成的。查看 [Angular官方文档](https://angular.io/cli)获取更多帮助。

### 开发环境配置

运行 `npm i` 安装项目依赖，运行 `ng serve` 启动开发服务器，在浏览器中输入 `http://localhost:4201/` 可以访问应用程序。可以实时更新代码。

### 打包部署

运行 `ng build` 命令打包项目。打包好的网页文件保存在 `dist/` 目录。
