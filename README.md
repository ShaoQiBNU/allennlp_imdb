allennlp的imdb实例
=========================

## Usage

There is a post about this repository: Click [this link](https://towardsdatascience.com/allennlp-startup-guide-24ffd773cd5b)

Running on CPU:

```bash
allennlp train \
    --include-package allennlp_imdb \
    -s /path/to/serialization \
    training_config/base_cpu.jsonnet
```

Running on GPU:

```bash
allennlp train \
    --include-package allennlp_imdb \
    -s /path/to/serialization \
    -o '{"trainer": {"cuda_device": 0}}' \
    training_config/base_cpu.jsonnet
```

Creating your own configuration file:

```
allennlp configure --include-package allennlp_imdb
```

## 另一个实例知乎详解和代码

https://zhuanlan.zhihu.com/p/73469009

https://github.com/allenai/allennlp-as-a-library-example
