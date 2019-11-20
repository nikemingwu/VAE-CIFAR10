# VAE-CIFAR10（代码整理中）
Requirements
===
	python 3
	TensorFlow = 1.14.0
	Numpy = 1.16.4
	keras = 2.2.4
	
Content
===
	cifar10_loader.py : 数据增强，对cifar数据进行预处理:剪裁、旋转、水平上下翻折等
	network.py : 有两个类，其中class VectorQuantizer是量化层，用来对隐变量进行字典学习。class VAE是网络模型，对输入的图像和标签通过字典学习的方式进行编码、解码。
	main.py : 获取cifar10_loader.py中的数据，学习network.py网络模型中的参数，每轮迭代之后在测试集上看训练的结果。
Usage
Usage
===
	只需要运行main.py文件，会自动在当前的目录下下载一个名字叫cifar-10-batches-bin的cifar-10的数据集，然后对网络模型进行训练和测试。
