# VAE-CIFAR10（代码整理中）
Requirements
===
	python 3
	TensorFlow = 1.14.0
	Numpy = 1.16.4
	keras = 2.2.4
	
Content
===
	cifar10_loader.py : 对cifar数据进行预处理，旋转、翻折等等
	main.py : 训练数据，保存模型参数等等
	network.py : 构造模型
Usage
===
	只需要运行main.py函数，会自动在当前的目录下下载cifar-10的数据集，然后训练模型
