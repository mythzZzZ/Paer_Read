DMFORMER CLOSING THE GAP BETWEEN CNN AND VISION TRANSFORMERS



创新点:

- 提出DMA机制
  - 提出Dynamic Multi-level Attention mechanism (DMA) （ 优于类似大小的视觉转换器 (ViT) 和卷积神经网络 (CNN)）
- 提出DMFormer的高效骨干网
- DMA替换自注意力机制
- DMFormer替换vision transformer 的结构









DMA

- 多尺度扩张卷积
- 轻量级门控机制提供输入适应性



![image-20230407091520466](https://zhangwenkang666.oss-cn-beijing.aliyuncs.com/image-20230407091520466.png)


$$
V =  ReLU(FC(GAP(X))
$$

$$
Attn = Sigmoid(FC(V))
$$

$$
Output = Attn \bigotimes Conv1 \times 1(X')
$$













DMFormer

![image-20230407094559615](C:/Users/Administrator/AppData/Roaming/Typora/typora-user-images/image-20230407094559615.png)











数据集：

- ImageNet-1K
- ADE20K