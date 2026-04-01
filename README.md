# 卡路里计算器

基于 USDA FoodData Central 真实数据的食物热量查询与累加工具，纯前端单页应用，无需安装任何依赖。

## 功能

- **真实数据**：所有热量数据来自 [USDA FoodData Central](https://fdc.nal.usda.gov/)，权威可靠
- **食物搜索**：实时查询 USDA 数据库，返回 kcal/100g 数据
- **自定义份量**：输入实际克数，自动计算热量并预览
- **热量累加**：多种食物叠加，实时显示今日总卡路里
- **数据类型筛选**：可按 Foundation / SR Legacy（基础食材）或 Branded（品牌商品）过滤结果

## 使用

直接用浏览器打开 `index.html` 即可，无需服务器。

```bash
git clone https://github.com/e-xianyu/calorie-god.git
cd calorie-god
open index.html   # macOS
# 或直接双击 index.html
```

## API Key

默认使用 `DEMO_KEY`，免注册，限额 1000 次/小时，日常使用足够。

如需更高频率，可在页面顶部替换为正式 Key：[免费申请 →](https://fdc.nal.usda.gov/api-key-signup/)

## 搜索建议

USDA 数据库为英文，**建议用英文搜索**，结果更准确：

| 中文 | 推荐搜索词 |
|------|-----------|
| 鸡胸肉 | `chicken breast` |
| 白米饭 | `white rice cooked` |
| 西兰花 | `broccoli` |
| 全脂牛奶 | `whole milk` |
| 鸡蛋 | `egg whole raw` |

## 数据来源

[USDA FoodData Central](https://fdc.nal.usda.gov/) — 美国农业部食物营养数据库，包含：

- **Foundation** — USDA 权威基础食材，数据最精确
- **SR Legacy** — 经典标准参考数据库
- **Branded** — 品牌商品，含包装食品标签数据
