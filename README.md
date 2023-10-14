# deep-learning
```bash
conda env create -f environment.yml

conda env export > environment.yml

conda env export --name <environment_name> > environment.yml
```
# 大模型时代，普通人的科研何去何从
## 王晋东不在家
1. 新的分析和评测

大模型时代显然需要新的分析和评测方法。不同于以往以公开测试集为准的机器学习，大模型现在可以将所有的公开数据集全部吃下（即overfit）。因此，不宜采用传统方式进行评测。可以思考：

更有难度、更符合人类标准的评测集是什么样的？
大模型的边界在哪里、什么样的数据可以测出来？
小模型和大模型到底有什么区别、仅仅是benchmark得分不同吗？
如何公平地评测不同大模型的能力？
到底何为”AGI“?如今的评测是否是AGI评测

2. 新的理论和方法

大模型对于做理论和基础研究的科研人员是个毁灭性的打击。原因很简单：深度学习理论在目前也无法很好地分析多层神经网络、更不必说更大、更不开源的黑盒大模型了。因此，理论研究人员可能会出现”巧妇难为无米之炊“的情形、不知道自己还能做什么。

但笔者认为，基础理论、数学、统计、概率等基础学科的重要性仍然无需多言，但需要结合大模型进行一些探索和突破。例如：

为什么CLIP仅采用image-text pair进行对比学习、泛化能力就很好？
如果是训练数据重要，那为何400M数据的CLIP和2B数据的Laion-CLIP在长尾数据上并没差太多？
数据、模型、算法、优化，哪个更重要？
如何加速大模型的训练，如从数据筛选、优化器更新的角度？

3. 更好的人与AI协同

既然打不过，那索性就加入。我们可以将大模型看作一次大的技术革命、一种新的人机交互方式。那么，此刻的你我就处于这种新的人机交互、人与AI协同的革命前夜，应该多去思考如何利用大模型的能力来做出更多变革：

如何提高写Prompt的能力、最好是自动写好的Prompt？
CV、NLP、Audio都有大模型，如何利用这些模型进行更好的多模态信息融合？
如何设计下一代人-AI协同交互的用户界面？
如何将大模型快速轻量地部署于端侧设备？

如何更轻量地微调大模型以服务于下游小数据领域？
<<<<<<< HEAD

4. 找大模型的短板
=======
4. 找大模型的短板、
>>>>>>> 
不得不说目前的大模型并不完美、其问题多多。笔者也在年初”卷“了一周、搞出了第一个ChatGPT的鲁棒性评测。我们发现大部分大模型其实对于对抗攻击并不鲁棒、其抗干扰能全力亟待提升。因此，一个自然的研究方向便是”找茬“：

大模型的OOD能力是不是够了？有大模型不需要OOD了？
大模型的长尾是不是做的很好了？这个笔者探索过了：显然不太行—Exploring vision-language models for imbalanced learning.
如何使大模型免受prompt injection、prompt leakage等攻击？
大模型生成内容如何判别是hallucination还是真的？

5. 更负责任、社会化的AI技术

新的技术革命需要新的社会变革，而变革的过程可能是充满荆棘的。好的研究视野应该放眼全社会、做出更负责任和更社会化的AI研究（Responsible AI, or societal AI），方可确保技术不被滥用、更好地服务人类：

如何进行有效的value alignment使AI准确地满足人的价值观？
如何对AI生成的内容进行有效监管使其实不被滥用？
如何分析生成式AI对教育、生产力、社会、心理学等诸多层面的影响？
新技术应该是”有温度“的：如何引导”前人“更加无痛地完成新技术的更迭？
此类问题的每一个都值得深入探讨。值得一提的是，笔者所在的研究组——微软亚洲研究院社会计算组的大部分研究人员均在做相关研究。也期待未来有更多的合作者加入进来一起合作。社会化问题任重而道远，需要跨学科、全社会的长期密切交流合作。
## 李沐团队:
- efficient (PEFT:parameter efficient fine tuning)
- existing stuff (pretrained model) new direction
- plug and play(即插即用)
- dataset, evaluation and survey
- 