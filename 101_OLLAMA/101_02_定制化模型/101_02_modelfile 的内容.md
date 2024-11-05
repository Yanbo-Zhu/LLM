
![](images/Pasted%20image%2020241105204101.png)

# 1 创造一个模型 

`ollama create <customized modelname> -f ./modelfile`

modelfile 是自己写的 

创建和运行模型：使用Ollama提供的命令行工具来创建和运行你的模型。
```bash
ollama create -f your_modelfile.yaml
ollama run gemma-custom-model
```




# 2 modelfile 的内容 

> 这个文件通常包含模型的基本信息，如模型类型、参数设置和任何特定的系统消息。


![](images/Pasted%20image%2020241105215440.png)





```
FROM: gemma:latest
PARAMETER:
  - temperature: 1
  - num_ctx: 4096
TEMPLATE: "完整的提示词模板"
SYSTEM:
  message: "自定义的系统消息"
```


设置参数：在Modelfile中，通过PARAMETER指令设置模型的各种参数，如温度和上下文窗口大小，以调整模型的行为。
定义提示模板：使用TEMPLATE指令定义模型的提示模板，这决定了模型如何响应用户的输入。


![](images/Pasted%20image%2020241105215502.png)


![](images/Pasted%20image%2020241105202702.png)



## 2.1 FORM

![](images/Pasted%20image%2020241105215612.png)



## 2.2 Parameter 


![](images/Pasted%20image%2020241105215630.png)


![](images/Pasted%20image%2020241105215640.png)


## 2.3 Template 

![](images/Pasted%20image%2020241105215706.png)


## 2.4 SYSTEM


![](images/Pasted%20image%2020241105215750.png)

## 2.5 ADAPTER

![](images/Pasted%20image%2020241105215757.png)

## 2.6 LICENSE


![](images/Pasted%20image%2020241105215805.png)


## 2.7 MESSAGE 


![](images/Pasted%20image%2020241105215836.png)

