## 🍽️ 饮食库
	- ### 安全可喂
	- {{query (and (page-property :type [[饮食]]) (page-property :安全等级 [[安全]]))}}
	  query-table:: true
	  query-properties:: [:page :食物类型 :年龄阶段 :alias]
	  query-sort-by:: 年龄阶段
	  query-sort-desc:: true
	- ### 需注意
	- {{query (and (page-property :type [[饮食]]) (page-property :安全等级 [[需注意]]))}}
	  query-properties:: [:page :食物类型 :年龄阶段 :alias]
	- ### 有毒
	- {{query (and (page-property :type [[饮食]]) (page-property :安全等级 [[有毒]]))}}
	  query-properties:: [:page :食物类型 :年龄阶段 :alias]
	- ### 绝对禁止
	- {{query (and (page-property :type [[饮食]]) (page-property :安全等级 [[绝对禁止]]))}}
	  query-properties:: [:page :食物类型 :年龄阶段 :alias]
	- ### 按食物类型
	- 水果: {{query (and (page-property :type [[饮食]]) (page-property :食物类型 [[水果]]))}}
	  query-properties:: [:page :安全等级 :年龄阶段 :alias]
	  query-sort-by:: 安全等级
	  query-sort-desc:: false
	- 蔬菜: {{query (and (page-property :type [[饮食]]) (page-property :食物类型 [[蔬菜]]))}}
	  query-properties:: [:page :安全等级 :年龄阶段 :alias]
	  query-sort-by:: 安全等级
	  query-sort-desc:: false
	- 种子粮: {{query (and (page-property :type [[饮食]]) (page-property :食物类型 [[种子粮]]))}}
	  query-properties:: [:page :安全等级 :年龄阶段]
	- 蛋白质食物: {{query (and (page-property :type [[饮食]]) (page-property :食物类型 [[蛋白质食物]]))}}
	  query-properties:: [:page :安全等级 :年龄阶段]
	- 加工食品: {{query (and (page-property :type [[饮食]]) (page-property :食物类型 [[加工食品]]))}}
	  query-properties:: [:page :安全等级 :年龄阶段 :alias]
- ## 🔬 营养成分
	- {{query (and (page-property :type [[营养成分]]))}}
	  query-properties:: [:page :营养素类型 :必需性]
	  query-sort-by:: page
	  query-sort-desc:: false
- ## 🏥 疾病与中毒
	- ### 按严重程度
	- 急症: {{query (and (page-property :type [[疾病]]) (page-property :严重程度 [[急症]]))}}
	  query-properties:: [:page :传染性 :病因类型 :受累系统 :好发年龄段 :alias]
	- 重症: {{query (and (page-property :type [[疾病]]) (page-property :严重程度 [[重症]]))}}
	- 中症: {{query (and (page-property :type [[疾病]]) (page-property :严重程度 [[中症]]))}}
	  query-properties:: [:page :传染性 :病因类型 :受累系统 :好发年龄段 :alias]
	- 轻症: {{query (and (page-property :type [[疾病]]) (page-property :严重程度 [[轻症]]))}}
	  query-properties:: [:page :传染性 :病因类型 :受累系统 :好发年龄段 :alias]
	- ### 按病因类型
	- 营养代谢性: {{query (and (page-property :type [[疾病]]) (page-property :病因类型 [[营养代谢性]]))}}
	  query-properties:: [:page :严重程度 :传染性 :受累系统 :好发年龄段 :alias]
	- 中毒性: {{query (and (page-property :type [[疾病]]) (page-property :病因类型 [[中毒性]]))}}
	  query-properties:: [:page :严重程度 :传染性 :受累系统 :好发年龄段 :alias]
- ## 🧠 行为习惯
	- {{query (property type [[行为]]) }}
	- _（尚待添加，欢迎贡献）_
- ## 🦴 身体构造
	- {{query (page-property :type [[身体构造]])}}
	  query-table:: true
	  query-properties:: [:page :隶属系统 :英文 :alias]
	  query-sort-by:: 隶属系统
	  query-sort-desc:: false
	- _（尚待添加，欢迎贡献）_
- ## 📝 文章
	- {{query (page-property :type [[文章]])}}
	  query-table:: true
	  query-properties:: [:page :文章分类 :alias]
	- _（尚待添加，欢迎贡献）_
- ## 🔄 生理周期
	- {{query (page-property :type [[生理周期]])}}
	  query-table:: true
	  query-properties:: [:block :page :周期类型 :持续时间 :触发因素 :alias]