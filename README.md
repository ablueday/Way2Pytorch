# Way2Pytorch
> 个人 Pytorch 学习笔记


pytorch 官网 https://pytorch.org/get-started/locally/

## 安装
[通过 conda 安装](https://pytorch.org/get-started/locally/#mac-anaconda)

1，创建环境

```conda create -n demo_pytorch```

2，安装 pytorch

```conda install pytorch torchvision -c pytorch```

3，测试

```
conda activate demo_pytorch # 激活刚才创建的环境
python # 打开 python

# 测试代码如下：
from __future__ import print_function
import torch
x = torch.rand(5, 3)
print(x)
```

```
# 得到类似下面的结果（一个 5 *3 的随机数矩阵）
tensor([[0.9729, 0.5000, 0.0495],
        [0.5766, 0.6751, 0.3493],
        [0.8237, 0.7004, 0.9541],
        [0.1875, 0.5825, 0.8255],
        [0.8927, 0.6136, 0.9592]])

```


----

## 参考

pytorch 英文教程 https://pytorch.org/tutorials/

pytorch 中文教程 https://pytorch.apachecn.org/#

pytorch 中文文档 https://pytorch-cn.readthedocs.io/zh/latest/

pytorch 教程集锦 https://github.com/amusi/PyTorch-From-Zero-To-One

卷积神经网络的卷积过程动图 https://github.com/vdumoulin/conv_arithmetic

斯坦福 CS231N 课程 http://cs231n.stanford.edu/

Neural Networks and Deep Learning http://neuralnetworksanddeeplearning.com/

卷积神经网络初学者指南 https://www.jiqizhixin.com/articles/2016-08-01-3

python 中的多线程和多进程 https://zhuanlan.zhihu.com/p/39542342


关于 python console 出错的解决方法 https://blog.csdn.net/qq_43275748/article/details/106375590

正确答案在评论里，抄写如下：

```
code = init.__code__
     args = [
           len(varnames),
           0,
           len(varnames),
           code.co_stacksize,
           code.co_flags,
           code.co_code,
           code.co_consts,
           code.co_names,
           varnames,
           code.co_filename,
           "__init__",
           code.co_firstlineno,
           code.co_lnotab,
           code.co_freevars,
           code.co_cellvars
       ]
       if sys.version_info >= (3, 8, 0):
           # Python 3.8 and above supports positional-only parameters. The number of such
           # parameters is passed to the constructor as the second argument.
           args.insert(2, 0)
       new_code = types.CodeType(*args)
   elif JYTHON:
       from org.python.core import PyBytecode
```

