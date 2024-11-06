
RAG 搜索增强功能 
更新大模型的 更新知识库 , 就不需要微调大模型了

# 1 RAG_Architecture_Workflow
 ![](images/Pasted%20image%2020241106105431.png)

RAG_Architecture
- 黄色 data loader 
    - 用于提取原始的数据 , 并且组成结构化的数据 , 存入向量数据库中
- 蓝色 data retriever 
    - 当用户触发一次 query, 就会向向量数据库中进行语义检索, 查出和用户问题相关的数据 , 
    - 按照相关性对数据进行排序
- 红色: LLM 作为最后结论生成的 generator 
    - LLM 会根据retrieve 查询的内容, 组成可以被人理解的reponse , 把结果返回给用户 


RAG_Workflow
- 数据载入和数据查询是并行的 
- 数据载入 
    - 原始图片 , 比如 网页, 邮件会通过数据处理的方式载入, 拆分成数据模块, 然后转换成Emdedding, 然后存入向量数据库当中 
    - Vector DB: 
        - Meta: face
        - klouma ?
- 数据查询 
    - 现将response经过语义转换, 通过 Vector DB Retrievaler 进行语义检索
    - 把检索到的数据, 放入已经编写好的 prompt 的模版当中, 制作成新的 prompt .
- 数据返回 
    - 当大语言模型 的检索完成, 将经过 prompt 处理的 response 返回给 用于 


