
相比其他开源框架，Torch 是一个非主流。

没错，说的就是它的开发语言：基于1990 年代诞生于巴西的 Lua，而非机器学习界广泛采用的 Python。
其实 Lua 和Python 都属于比较容易入门的语言。但后者明显已经统治了机器学习领域，尤其在学界。
而企业界的软件工程师最熟悉的是 Java，对 Lua 也比较陌生。这导致了 Torch 推广的困难。
因此，虽然 Torch 功能强大，但并不是大众开发者的菜。

那么它强大在哪里？

首先，Torch 非常适用于卷积神经网络。它的开发者认为，Torch 的原生交互界面比其他框架用起来更自然、更得心应手。

其次，第三方的扩展工具包提供了丰富的递归神经网络（ RNN）模型。

因为这些强项，许多互联网巨头开发了定制版的 Torch，以助力他们的 AI 研究。这其中包括 Facebook、Twitter，和被谷歌招安前的 DeepMind。

与 Caffe 相比，在 Torch 里定义一个新层级比它要容易，因为你不需要写  C++ 代码。
和 TensorFlow 和 Theano 比起来，Torch 的灵活度更高，
因为它是命令式的；而前两者是陈述式的（declarative），你必须 declare 一个计算图。
这使得在 Torch 上进行束搜索（beam search）这样的操作要比它们容易得多。

Torch 的热门应用：在增强学习领域，用卷积神经网络和代理处理图像问题。

兴趣主要在增强学习的开发者， Torch 是首选。

优点：
灵活度很高

高度模块化

容易编写你自己的层级

有很多训练好的模型

缺点：
需要学  Lua

通常需要自己写训练代码

不适于循环神经网络

没有商业支持


[![Join the chat at https://gitter.im/torch/torch7](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/torch/torch7?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![Build Status](https://travis-ci.org/torch/torch7.svg)](https://travis-ci.org/torch/torch7)

## Need help? ##

* Questions, Support, Install issues: [Google groups](https://groups.google.com/forum/#!forum/torch7)
* Reporting bugs: [torch7](https://github.com/torch/torch7/issues) [nn](https://github.com/torch/nn/issues) [cutorch](https://github.com/torch/cutorch/issues) [cunn](https://github.com/torch/cutorch/issues) [optim](https://github.com/torch/optim/issues) [threads](https://github.com/torch/threads/issues)
* Hanging out with other developers and users (strictly no install issues, no large blobs of text): [Gitter Chat](https://gitter.im/torch/torch7)

<a name="torch.reference.dok"></a>
# Torch Package Reference Manual #

__Torch__ is the main package in [Torch7](http://torch.ch) where data
structures for multi-dimensional tensors and mathematical operations
over these are defined. Additionally, it provides many utilities for
accessing files, serializing objects of arbitrary types and other
useful utilities.

<a name="torch.overview.dok"></a>
## Torch Packages ##

  * Tensor Library
    * [Tensor](doc/tensor.md) defines the _all powerful_ tensor object that provides multi-dimensional numerical arrays with type templating.
    * [Mathematical operations](doc/maths.md) that are defined for the tensor object types.
    * [Storage](doc/storage.md) defines a simple storage interface that controls the underlying storage for any tensor object.
  * File I/O Interface Library
    * [File](doc/file.md) is an abstract interface for common file operations.
    * [Disk File](doc/diskfile.md) defines operations on files stored on disk.
    * [Memory File](doc/memoryfile.md) defines operations on stored in RAM.
    * [Pipe File](doc/pipefile.md) defines operations for using piped commands.
    * [High-Level File operations](doc/serialization.md) defines higher-level serialization functions.
  * Useful Utilities
    * [Timer](doc/timer.md) provides functionality for _measuring time_.
    * [Tester](doc/tester.md) is a generic tester framework.
    * [CmdLine](doc/cmdline.md) is a command line argument parsing utility.
    * [Random](doc/random.md) defines a random number generator package with various distributions.
    * Finally useful [utility](doc/utility.md) functions are provided for easy handling of torch tensor types and class inheritance.

<a name="torch.links.dok"></a>
## Useful Links ##

  * [Community packages](https://github.com/torch/torch7/wiki/Cheatsheet)
  * [Torch Blog](http://torch.ch/blog/)
  * [Torch Slides](https://github.com/soumith/cvpr2015/blob/master/cvpr-torch.pdf)

