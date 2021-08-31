# paper-of-pruning


## saliency-based方法
### 按重要性排序，将不重要的部分去除
* <Pruning Filters for Efficient ConvNets>
* <Learning Structured Sparsity in Deep Neural Networks>
* <Sparse Convolutional Neural Networks>
* <Learning Efficient Convolutional Networks Through Network Slimming>
* <Network Trimming: A Data-Driven Neuron Pruning Approach towards Efficient Deep Architectures>

### ‘smaller-norm-less-important’准则未必成立
* <Rethinking the Smaller-Norm-Less-Informative Assumption in Channel Pruning of Convolution Layers>
* <Pruning Convolutional Neural Networks for Resource Efficient Transfer Learning> 
* <SNIP: Single-shot Network Pruning based on Connection Sensitivity>


### 最小化裁剪后网络对于特征输出的重建误差
* <ThiNet: A Filter Level Pruning Method for Deep Neural Network Compression> 
* <Channel pruning for accelerating very deep neural networks> 
* <NISP: Pruning Networks using Neuron Importance Score Propagation>
* <Discrimination-aware Channel Pruning for Deep Neural Networks>

### 基于其它的准则对权重进行重要性排序
* <Filter Pruning via Geometric Median for Deep Convolutional Neural Networks Acceleration>

##考虑参数间的相互关系，试图找导全局更优解

### 离散空间下的搜索
* <Structured Pruning of Deep Convolutional Neural Networks>
* <N2N Learning: Network to Network Compression via Policy Gradient Reinforcement Learning>

### 规划问题
* <Collaborative Channel Pruning for Deep Networks>

### Bayesian方法
* <Variational Dropout Sparsifies Deep Neural Networks>

### 基于梯度的方法
* <Learning Sparse Neural Networks through L0 Regularization>

### 基于聚类的方法
* <SCSP: Spectral Clustering Filter Pruning with Soft Self-adaption Manners>
* <Exploring Linear Relationship in Feature Map Subspace for ConvNets Compression>

## Sparsity Ratio
sparsity ratio定义为层中为0参数所占比例.Predefined方法由人工指定每一层的比例进行裁剪，因此目标结构是提前确定。而automatic方法会根据所有的layer信息（即全局信息）由pruning算法确定每层裁剪比例，因此目标结构一开始并不确定。

### predifined
* <MobileNets: Efficient Convolutional Neural Networks for Mobile Vision Applications> 
* <EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks>
* <Learning both Weights and Connections for Efficient Neural Networks>
* <Pruning Filters for Efficient ConvNets>

### automatic
* <Learning Efficient Convolutional Networks through Network Slimming>
* <Play and Prune: Adaptive Filter Pruning for Deep Model Compression>
* <ADC: Automated Deep Compression and Acceleration with Reinforcement Learning>
* <“Learning-Compression” Algorithms for Neural Net Pruning>

## 精度恢复
training，pruning，fine-tuning三段式。后面两个阶段交替进行，每次pruning后损失的精度可以由后面的fine-tuning来弥补，该过程也称为iterative pruning。
* <Channel Pruning for Accelerating Very Deep Neural Networks>
* <To Prune, or Not to Prune: Exploring the Efficacy of Pruning for Model Compression>

## 重新审视假设
over-parameterization对训练是否真的那么有益，还有原网络的权重是否在pruning中很重要。
* <The Lottery Ticket Hypothesis: Finding Sparse, Trainable Neural Networks>
* <Rethinking the Value of Network Pruning>

