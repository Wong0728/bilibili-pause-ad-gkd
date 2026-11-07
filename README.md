# bilibili-pause-ad-gkd

哔哩哔哩「视频页暂停广告」屏蔽规则（GKD 订阅）。

自动处理播放器上出现的「X秒后将展示广告」倒计时与暂停页广告卡片：
弹出即自动关闭，不再手动点。

## 订阅方式

1. 复制订阅链接：

   ```
   https://raw.githubusercontent.com/Wong0728/bilibili-pause-ad-gkd/main/gkd.json5
   ```

2. 打开 GKD App → 订阅 → 右上角「+」→ 粘贴链接 → 添加。

或在手机浏览器点击一键导入：

```
gkd://subscription/import?url=https%3A%2F%2Fraw.githubusercontent.com%2FWong0728%2Fbilibili-pause-ad-gkd%2Fmain%2Fgkd.json5
```

## 包含规则

| 组 | 说明 | 默认 |
| --- | --- | --- |
| 局部广告-播放器广告倒计时-自动取消 | 倒计时条出现时自动点「取消」，阻止广告弹出 | 开 |
| 局部广告-暂停页广告-自动关闭 | 广告卡片弹出时自动点右上角 X 关闭 | 开 |
| 分段广告-暂停页广告-自动屏蔽 | 自动点「不感兴趣」并选择屏蔽原因 | 关（与上一组二选一） |

## 更新

规则文件内置 `updateUrl`，GKD 会自动检查并更新；手动更新可在 GKD 订阅页下拉刷新。

## 声明

规则基于 GKD 快照与控件树验证生成，B 站版本更新后选择器可能失效，欢迎提 issue。
仅供学习交流，请勿用于商业用途。
