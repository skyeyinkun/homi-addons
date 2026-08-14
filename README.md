# HOMI Add-ons

HOMI 的 Home Assistant Add-on 官方安装仓库。此仓库只提供安装配置、用户文档与运行镜像分发，不包含开发源码。

## 安装

1. 打开 Home Assistant，进入 **设置 → 加载项 → 加载项商店**。
2. 点击右上角 **⋮ → 仓库**，添加：

   ```text
   https://github.com/skyeyinkun/homi-addons
   ```

3. 在商店中找到 **HOMI**，点击 **安装** 并启动。
4. 从 HA 左侧栏点击 **HOMI**，或在加载项页面选择 **打开 Web UI**。

## 首次激活

1. 在 HOMI 授权页复制申请码并发送给授权签发方。
2. 收到有效授权码后粘贴激活。
3. 刷新设备列表，按需整理房间、常用设备、AI 服务和首页布局。

## 访问与安全

- 推荐使用 Home Assistant Ingress（HA 左侧栏或“打开 Web UI”）。
- 可信局域网也可访问 `http://HA主机IP:8099/`。
- `8099` 不经过 Home Assistant 登录页；仅限可信局域网使用，禁止进行路由器端口转发或通过公网反向代理暴露。

## 当前版本

当前版本为 [HOMI 1.0.0](homi_dashboard/CHANGELOG.md)。

## 授权

一份授权绑定一台运行 HOMI 的 Home Assistant 主机。同一已授权实例可供家庭内多台终端使用。HOMI 是 Home Assistant 生态的第三方软件，不代表 Home Assistant 官方背书、认证或支持。
