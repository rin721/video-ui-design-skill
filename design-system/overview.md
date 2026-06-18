# 设计系统总览

## Aesthetic Style

```yaml
aesthetic_style:
  style_name: "Soft Signal Interface"
  visual_personality:
    - "轻盈"
    - "友好"
    - "有秩序"
    - "内容优先"
    - "克制但有表达"
  mood_keywords:
    - "低噪音"
    - "高清晰度"
    - "柔和能量"
    - "结构化温度"
    - "轻微动势"
  composition_traits:
    - "固定工具导航围绕灵活内容区"
    - "首屏为身份、搜索或产品语境提供清晰入口"
    - "用宽外边距平衡密集卡片网格"
    - "区块标签可搭配紧凑计数或状态标记"
    - "主扫描路径从语境到网格再到详情"
  surface_traits:
    - "近白页面画布"
    - "内容需要收束时使用半透明抬升面"
    - "active 导航和 focus 使用柔和强调色"
    - "细边框和低层级阴影"
  detail_traits:
    - "圆角媒体卡片"
    - "圆形图标控件"
    - "短标签配合强色彩强调"
    - "metadata 使用小图标或紧凑文本分组"
  suitable_site_types:
    - personal_homepage
    - blog
    - community
    - saas
    - portfolio
    - ecommerce
    - documentation
  avoid:
    - "厚重界面框架"
    - "装饰堆叠"
    - "低对比粉彩文字"
    - "在工具型界面中放置过大的营销卡片"
    - "缺少中性色和辅助色平衡的单色页面"
```

## System Intent

构建易接近、直接、便于扫描的页面。用柔和颜色标记重要操作，而不是装饰每个表面。内容卡片应保持轻量，让图片、标题和 metadata 承担页面节奏。

## Reusable Pattern

使用持久导航层、清晰内容标题、响应式网格或页面外壳，以及可见行动路径。在紧凑屏幕中，将主导航移入底部栏或顶部操作行，并根据可用宽度保持一列或两列卡片。
