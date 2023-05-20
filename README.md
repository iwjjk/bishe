# 基于注意力机制的花朵图像分类算法
项目包括三个文件,包含了三个不同的算法，分别是Vision Transformer,Swin Transformer以及MobileViT,三个算法的总体结构一致，运行方式如下所述
# 代码运行方式介绍
1.下载数据集，代码中默认使用花朵数据集  
2.在train.py脚本修改正确数据集的路径  
3.下载想使用的预训练权重模型  
4.在train.py中将--weights参数设置成下载好的预训练权重路径  
5.使用train.py脚本开始训练了，训练过程中会自动生成class_indices.json文件  
6.此时模型就已经训练完毕，可以使用tensorboard查看训练集与测试集的准确率变化  
7.在predict.py脚本中将model_weight_path设置成训练好的模型权重路径(默认保存在weights文件夹下)   
8.在predict.py中将img_path设置为你想预测图片的绝对路径，这样就可以用predict.py脚本进行预测了  
9.其他数据集可以将训练和预测脚本中的num_classes设置为此数据集的类别数  
