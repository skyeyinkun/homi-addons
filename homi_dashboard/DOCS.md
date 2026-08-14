# HOMI

HOMI 是运行在 Home Assistant 本地环境中的家庭控制面板，用于在一个界面中查看和控制已接入 Home Assistant 的设备，并提供房间管理、自动配置、AI 助手、授权和本地备份能力。

## 安装

1. 打开 Home Assistant，进入 **设置 → 加载项 → 加载项商店**。
2. 点击右上角 **⋮ → 仓库**，添加 HOMI 分发仓库地址。
3. 在商店中找到 **HOMI**，点击 **安装** 并启动。
4. 通过 HA 左侧栏或 **打开 Web UI** 进入 HOMI。

## 首次激活

1. 在 HOMI 授权页复制申请码并发送给授权签发方。
2. 收到有效授权码后粘贴激活。
3. 刷新设备列表，按需要整理房间、常用设备、AI 服务和首页布局。

## 访问方式

- 推荐使用 Home Assistant Ingress（HA 左侧栏或“打开 Web UI”）。
- 可信局域网也可访问 `http://HA主机IP:8099/`。
- `8099` 不经过 Home Assistant 登录页；仅限可信局域网使用，禁止进行路由器端口转发或通过公网反向代理暴露。

## 数据与安全

- Add-on 通过 Home Assistant Supervisor 运行时令牌连接当前 Home Assistant，不要求用户创建长期访问令牌。
- HOMI 配置、授权与可选 AI 服务配置保存在安装它的 Home Assistant 主机上。
- AI 功能需要用户自行配置兼容 OpenAI 接口的模型服务；请自行确认服务商的费用、隐私与可用性。
- 更新、重装或调整重要配置前，请先创建 Home Assistant 原生备份。HOMI 内置备份仅作为额外副本，不替代 HA 原生备份。

## 授权

一份授权绑定一台运行 HOMI 的 Home Assistant 主机。同一已授权实例可供家庭内多台终端使用。HOMI 是 Home Assistant 生态的第三方软件，不代表 Home Assistant 官方背书、认证或支持。
