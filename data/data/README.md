# 数据集说明

## 目录

```
.
└── data
    ├── wos_label_desc.json
    ├── wos_prob_child_parent.json
    ├── wos_prob.json
    ├── wos.taxnomy
    ├── wos_test.json
    ├── wos_train.json
    └── wos_val.json
```

## Label

| 文件名                          | 用途                    |
|------------------------------|-----------------------|
| `wos.taxnomy`                | 描述 Label 的层级结构        |
| `wos_label_desc.json`        | Label 本身的描述信息（文本）     |
| `wos_prob.json`              | Label 先验概率（上层 → 下层）   |
| `wos_prob_child_parent.json` | Label 的父节点关系（下层 → 上层） |

## 语料
| 文件名                          | 用途                    |
|------------------------------|-----------------------|
| `wos_train.json`             | 训练集                   |
| `wos_val.json`               | 验证集                   |
| `wos_test.json`              | 测试集                   |

每行是一个 dict，注意：文件整体不是 json 格式。每行包含 2个字段，`token` 是 List of str，`label` 是 list of str.
