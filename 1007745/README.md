# 圣剑启示录宣传页

- 官网：https://wt8930419-ai.github.io/xianmeng-games/1007745/
- 官方资料：https://www.taptap.cn/app/1007745
- 按用户最终要求只展示一个移动端入口，按钮和二维码共用 `site-config.json` 的 `taptap_url`；未配置 PC 独立入口。
- 官方素材、原始尺寸和无损转码记录在 `media/sources.json`，原始 PNG 候选保留于项目 `logs/1007745-originals/`。
- 下载、测试及游戏开放状态以官方 TapTap 页面为准。

页面源文件为 `tools/index.template.html`，不要直接维护生成的 `index.html`。从仓库根目录运行 `python 1007745/tools/prepare_site.py` 重新生成页面和二维码，运行 `python tools/preview_site.py` 后访问 http://127.0.0.1:8766/1007745/ 。

REP 官网品牌挂件填写本游戏独立官网地址。发布验证不代表 REP 已提交或审核通过。
