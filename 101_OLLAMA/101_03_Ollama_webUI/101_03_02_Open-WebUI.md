
https://github.com/open-webui/open-webui


# 1 account

Name: Ya*** Z**
Email: bigberlin200
密: `B*****10***


# 2 Installation
## 2.1 Installation via Python pip

Open WebUI can be installed using pip, the Python package installer. Before proceeding, ensure you're using **Python 3.11** to avoid compatibility issues.

1. **Install Open WebUI**: Open your terminal and run the following command to install Open WebUI:
    ```shell
    pip install open-webui
    ```

**Running Open WebUI**: After installation, you can start Open WebUI by executing:
```shell
open-webui serve
```

This will start the Open WebUI server, which you can access at [http://localhost:8080](http://localhost:8080)

### 2.1.1 error : python 3.12 不可用 
https://github.com/open-webui/open-webui/discussions/2596
We only support Python 3.11, and recommend using a virtual environment tool such as Conda.


解决方式 
In arch I am using `pipx install --fetch-missing-python --python 3.11 open-webui` command to install it.



## 2.2 Installation via docker  (我用的是这种中方式 )

If Ollama is on your computer, use this command:
```
docker run -d -p 3000:8080 --add-host=host.docker.internal:host-gateway -v open-webui:/app/backend/data --name open-webui --restart always ghcr.io/open-webui/open-webui:main
```




# 3 访问 webui 

you can access at [http://localhost:8080](http://localhost:8080)



# 4 管理模型 下载模型 


![](images/Pasted%20image%2020241106120952.png)



在 "Ollama.com 拉去 一个模型" 中输入    https://ollama.com/library 找到的模型的名字 
![](images/Pasted%20image%2020241106121121.png)









