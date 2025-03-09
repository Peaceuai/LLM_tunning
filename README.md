# ollama，open-webui安装
ollama安装为了能够拉取我们微调好的大模型到本地，open-webui则是以图形化界面的方式提供给我们跟AI交互

## ollama安装
下载地址：https://ollama.com/
![image](https://github.com/user-attachments/assets/c7edab6b-21bc-424b-af6c-c743992bdf76)
![image](https://github.com/user-attachments/assets/2a16ea46-20bd-4d6e-a49f-b360d42a740d)
等待一会下载成功之后，双击安装即可

打开cmd，输入
ollama -v
如果有显示版本信息则证明安装成功

后面拉取微调之后的模型用这个命令
ollama pull hf.co/{用户名}/{模型名}

## open-webui安装
安装open-webui前，先安装conda，安装一个miniconda就行了
下载conda地址：https://www.anaconda.com/download/success
![image](https://github.com/user-attachments/assets/3a8705a6-716b-4d4a-87a1-3ea5884d6ced)
安装的时候记得选上配环境变量

有安装conda的，无论是正常的还是mini的，cmd输入conda -v看看有没有配置环境变量
没有的根据下面教程配一下
https://blog.csdn.net/yinjun3215/article/details/123705879

conda配置完成了之后，在cmd输入
conda create -n {虚拟环境名称} python=3.11
这样虚拟环境就创建完成，之后继续在cmd输入
pip install open-webui
这样open-webui环境安装完成
之后继续在cmd输入
open-webui serve
服务启动完成，通过浏览器http://localhost:8080访问


























## Install requirements

```python
pip install requirements.txt
```

## Running the mode of training to get the agent file

```python
python Q_learning.py t
```

## Running the mode of showing to show the performance by the agent

```python
python Q_learning.py p
```

## Results

 The below picture is about the process of training
 ![image](https://github.com/user-attachments/assets/313e58ba-50f5-4558-b832-2456c63b8001)

 The below picture is about the performance by the agent
 ![image](https://github.com/user-attachments/assets/d350aaa7-9d81-42f9-8821-f6b78c2a557c)

## Reference

https://github.com/kevinunger/snake-Q-Learning
