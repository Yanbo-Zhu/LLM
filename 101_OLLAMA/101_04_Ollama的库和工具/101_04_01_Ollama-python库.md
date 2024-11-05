
Ollama-python库是为Python开发者提供的，用于与Ollama服务进行交互的工具。这个库使得Python开发者能够轻松地在他们的项目中集成和运行大型语言模型。
主要功能

    模型管理：通过Python脚本管理模型的创建、拉取、删除和复制。
    模型运行：在Python环境中运行Ollama模型，并处理模型的输入输出。
    自定义模型：支持通过Python脚本自定义模型参数和行为。


pip install ollama-python


# 1 例子

```
from ollama_python import OllamaClient

client = OllamaClient("http://localhost:11434")

# 创建模型
client.create_model("my_model", "path/to/modelfile")

# 运行模型
response = client.run_model("my_model", "Hello, world!")
print(response)

```


---

![](images/Pasted%20image%2020241105215243.png)







