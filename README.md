#   电力领域中文分词模型
ecws　是面向电力领域的基础中文分词模型组件，目标是打造电力领域的自然语言处理基础能力

## 安装指南
ecws 依赖以下包:

+ torch==1.5.1
+ allennlp==1.0.0


## 版本号
```version
R3.0.1
```

## 模型命名
    NLP-ECWS-R3.0.1

## 安装

* 第一步，安装 ecws

	使用 pip 安装

	```
	$ pip install ecws
	```
	或从源代码安装

	```
    git clone https://github.com/rises-tech/ecws.git
    cd NLP-ECWS-R3.0.1
    pip install -e .
    ```
 
下载`ecws.model`文件，后续提供

python引用方式：

```python

from ecws.segment import Segmenter

model_path = 'ecws.model'

predict = Segmenter(model_path)

d = predict.seg(sent)
```

其中返回的结果是一个字典，字段'sent'中包含分词结果。


## 开发者
张强<<[alxor@live.cn](alxor@live.cn)>>


