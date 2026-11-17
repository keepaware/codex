# 验收记录

- schema v2 goal spec 校验通过。
- 浏览器实际逐页打开15页；JavaScript错误0，文本块越界0；检查了页面缩略图与报价、公司介绍、收益等重点页。
- 原版 Swiss 校验器未兼容无 layout 字段的 bespoke 页面；原版 copy 校验器未物化 schema v2 structure 投影、且误报显式空白的可选槽。
- 本地兼容校验使用同一运行时 materializer 解析结构投影、承认明确声明的 bespoke 页面，并仅对投影中显式生成的空白槽免除默认文案误报。资源、来源、未知布局、默认文案与内容校验仍保留。
- 兼容后的 Swiss 与 copy 校验均通过；未改动主题组件或运行时渲染逻辑。
