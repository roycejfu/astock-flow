# A股资金流向日报 · GitHub Pages

每个交易日 19:00 自动生成 A股资金流向看板并发布到本页面。

## 网址

**https://roycejfu.github.io/astock-flow/**

## 内容

- 四大指数行情（上证/深证成指/创业板指/科创50）
- 指数资金流向（超大单/大单/中单/小单）
- 25+ 行业板块资金流向（主力净流入、5日/20日涨跌、换手率）
- 个股资金流向详情（主力净流入 TOP 板块内个股）
- 外围市场（美股/港股/日韩/黄金/原油）
- 市场宽度（涨跌家数、涨停跌停、成交额）

## 目录结构

```
flow-site/
├── index.html        # 首页（最新看板 + 历史列表）
├── latest.html       # 最新一期看板
├── archive/          # 历史看板归档 YYYY-MM-DD.html
├── meta.txt          # 每期标题/资金趋势
└── publish.py        # 发布脚本
```

## 发布命令

```bash
python3 publish.py --report /path/to/a股资金流向看板.html \
                   --date YYYY-MM-DD \
                   --title "一句话摘要" \
                   --trend up|down|mixed
```
