
# 1 Ollama 的命令 



```

# 查看版本
ollama -v 

# 下载模型 
ollama pull llama3:2b

# 直接运行(不推荐)
ollama run llama3.1 

# 查看某个模型具体的描述 
ollama show llama3:2b
ollama show llama2:latest --modelfile > myllama2.modelfile


# 查看安装目录 
ll -h ~/.ollama/ 

# 列出模型
ollama ls 

# 删除模型 
ollama rm komamodel 

# 拷贝模型 
ollama cp llama3.1:8b my-model-test    

```


访问模型库
Ollama的模型库包含了多种预训练的大型语言模型，用户可以根据自己的需求选择合适的模型。以下是访问模型库的步骤：
- 查看模型列表：使用`ollama models`命令可以列出所有可用的模型。
- 获取模型详情：对于特定的模型，你可以使用`ollama model details [模型名称]`来获取更详细的模型信息，包括模型的描述、版本、大小等。
- 下载模型：使用`ollama download [模型名称]`命令来下载模型到本地。
- 更新模型：定期检查模型库中的更新，使用`ollama update [模型名称]`来更新已下载的模型。

自定义模型

Ollama允许用户根据自己的需求对模型进行自定义。这包括调整模型的参数、添加特定的数据集或修改模型的结构。以下是自定义模型的基本步骤：

选择基础模型：首先，从模型库中选择一个基础模型作为自定义的起点。

- 调整参数：使用`ollama customize [模型名称] --params [参数设置]`命令来调整模型的参数。例如，你可以调整模型的学习率、批量大小等。
- 训练模型：如果你有特定的数据集，可以使用`ollama train [模型名称] --dataset [数据集路径]`命令来训练模型。
- 验证和测试：训练完成后，使用`ollama test [模型名称]`命令来验证模型的性能。


## 1.1 list 

查看下载的 model

![](images/Pasted%20image%2020241105201716.png)


## 1.2 show 
![](images/Pasted%20image%2020241105205721.png)



# 2 模型本身的命令 


```
# 查看帮助 
/? 

# 显示 modelfile 中写入的系统提示 
/show system 

# 退出模型 
执行 /exit
```


## 2.1 /show
![](images/Pasted%20image%2020241105210029.png)

