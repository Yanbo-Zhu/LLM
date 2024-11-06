

# 1 Example1

本地 pdf 作为额外的数据源 

https://www.youtube.com/watch?v=HtqmEREAPC0&list=PL1Jq_JipFh5i38FOY0IFGtxfdhZBQPKBQ

- Ingeration tool 
    -  langchain: 
- VectorDB
    - Chroma DB 
- loading local LLM 
    - Ollama: 
- Frontend UI
    - Gradio 


![](images/Pasted%20image%2020241106112201.png)



## 1.1 代码 

1. 载入数据
2. 接受输入的问题和查询
3. 返回结果给LLM
4. LLM组织输出给用户 


![](images/Pasted%20image%2020241106113219.png)

![](images/Pasted%20image%2020241106114341.png)

Function: loadDataFromPDFFile
```
filter_complex_metadat: 代表去除pdf 中的一些 metadata
然后存入 vector_stroe
```


Function: modelResponse
 - retriever (row 42)
     - k: 在参选候选集里面, 选多少个结果返回给其他的程序代码 
 - hpCahin: 
     - 创建一个Chain 
     - 使用 LCEL: longchain expression language 



Function: main
- 把回复的函数关联到 Gradio UI 的 interface 中 
- 然后launch 这个 UI 


# 2 Example 


- GPT4ALL
- Jan
- LM Studio 
- Anything LLM






