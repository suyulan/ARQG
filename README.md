## ARQG

ARQG是一个应用于问题生成任务的大规模迁移学习数据集。
ARQG来源于答案选择和阅读理解开源数据集，其具体数据来源如表1所示。

<img width="553" alt="table1" src="https://user-images.githubusercontent.com/55616659/115717319-a7367b00-a3ac-11eb-8f53-860c32f9a220.png">

为了使构造的ARQG数据集能较好地针对问题生成任务，我们对不同长度量级句子的最大长度以及不同类型数据之间的比例进行了控制，其详细数据信息如表2所示。

<img width="459" alt="table2" src="https://user-images.githubusercontent.com/55616659/115717358-aef61f80-a3ac-11eb-87f5-c1702fd227a0.png">


ARQG.zip包含如下文件: 

—— ARQG-train.json

—— ARQG-dev.json

其具体格式如下所示，每行为json格式，包含“src”和“tgt”两个字段，“src”表示源端陈述句（若陈述句中出现“[SEP]”，则表示“[SEP]”前为陈述句部分，“[SEP]”后为答案部分），“tgt”表示目标疑问句。

```json
{"src": "( CNN ) -- No one expected to find Donna Molnar alive . [SEP] Donna Molnar", "tgt": "Who went missing?"}
{"src": "the film is being released on august 17 , 2018 .", "tgt": "when is the little mermaid live action movie coming out"}
```
