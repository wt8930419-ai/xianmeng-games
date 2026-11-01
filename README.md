# 仙梦游戏官网

仙梦游戏的独立官网仓库。根首页为游戏导航，游戏按 TapTap App ID 放入独立目录，目前展示《圣剑启示录》和《模拟三国城》。

| 页面 | 目录 | 公开地址 |
| --- | --- | --- |
| 仙梦游戏官网 | `/` | https://wt8930419-ai.github.io/xianmeng-games/ |
| 圣剑启示录 | `1007745/` | https://wt8930419-ai.github.io/xianmeng-games/1007745/ |
| 模拟三国城 | `818856/` | https://wt8930419-ai.github.io/xianmeng-games/818856/ |

- 仓库：https://github.com/wt8930419-ai/xianmeng-games
- 发布源：GitHub Pages，`main` 分支根目录 `/`。
- 厂商主页：https://www.taptap.cn/developer/224656
- 《圣剑启示录》按用户最终要求展示一个移动端 REP 入口，按钮和二维码读取 `1007745/site-config.json` 的 `taptap_url`。
- 《模拟三国城》仅展示安卓 REP 入口，按钮和二维码均读取 `818856/site-config.json` 的 `taptap_url`。
- 《模拟三国城》的页面及官方素材从 `game-showcase` 的提交 `f3d254758efdf29df8559b62323f1574dd0e6a20` 迁入，素材来源见 `818856/media/sources.json`。
- 原官网地址 `https://wt8930419-ai.github.io/game-showcase/818856/` 仅保留跳转；REP 官网资源应改填新独立官网地址，提交与审核状态以 REP 后台为准。

## 本地维护

修改 `818856/tools/index.template.html` 或下载配置后重新生成，不直接维护生成的 `index.html`。

```powershell
python -m pip install -r 818856/tools/requirements.txt
python 818856/tools/prepare_site.py
python tools/preview_site.py
```

预览首页：http://127.0.0.1:8766/ ，游戏页：http://127.0.0.1:8766/818856/ 。未来仙梦游戏的作品在本仓库内新增独立目录与首页入口，不加入 won＊的工作室的 `game-showcase` 仓库。
