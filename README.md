# 午夜便利店 · Night Shift

一个全中文的浏览器经营小游戏。玩家经营一间深夜便利店，在三分钟营业时间内完成顾客订单、控制库存、处理随机事件并升级店铺。

## 本地运行

```bash
node server.cjs
```

打开 http://127.0.0.1:4173/ 。

## Docker

构建并运行：

```bash
docker build -t wuyegame .
docker run --rm -p 8080:80 wuyegame
```

打开 http://127.0.0.1:8080/ 。

推送到 main 后，GitHub Actions 会构建并发布：

```text
ghcr.io/handwish-max/wuyegame:latest
ghcr.io/handwish-max/wuyegame:<commit-sha>
```

仓库同时包含 GitHub Pages 部署工作流。首次使用时，在仓库 Settings → Pages → Build and deployment 中选择 GitHub Actions。

## 玩法

- 点击商品加入购物篮，再次点击可以撤回
- 按顾客订单拿齐商品后结账
- 顾客耐心耗尽前完成服务
- 使用营业额补货和升级咖啡机、货架、霓虹灯牌
- 留意暴雨夜、深夜赶工潮和午夜电波等随机事件
- 三分钟结束后根据营业额、服务人数、口碑和目标完成情况获得评级
