# 皇家月子中心服务合约

在线表单 + PDF 导出工具。基于原版 [netfunbot.github.io/yzzx/johnny.html](https://netfunbot.github.io/yzzx/johnny.html) 改造。

## 部署

- **GitHub Pages**: https://netfunbot.github.io/johnny/johnny.html (推送 `main` 分支后自动生效)
- 源文件: `johnny.html` (单文件,无依赖)

## 改动

相对原站,把「二、月子中心服务明细」整张表全部抽出成可编辑输入框:

- A 住宿 (A1, A2, A3) — 默认值 = 原站预设文字
- B 膳食 (B1, B2, B3, B5, B6) — 默认值 = 原站预设文字
- D 妈咪照顾 (D1, D2, D3, D4) — 默认值 = 原站预设文字
- E 其他免费服务 (E1, E2, E3, E4, E5, E6) — 默认值 = 原站预设文字,E6 留空时不显示该行

其他字段(合约编号、甲方乙方信息、费用档位、签字日期)与原站一致。

## 部署步骤

```bash
# 一次性
git remote add origin https://github.com/netfunbot/johnny.git
git push -u origin main

# GitHub Settings → Pages → Source: main / (root)
```

## 修改后再部署

```bash
# 编辑 johnny.html 后:
git add johnny.html
git commit -m "update"
git push
```

GitHub Pages 30 秒内自动生效。