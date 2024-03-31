Thank you for your comprehensive review and the insights provided. We are particularly grateful for your recognition of our intensive experimentation efforts and the aesthetic appeal of our figures. The novelty of our approach and its potential contributions are areas we are eager to refine and elaborate on, based on your feedback.

**Reproducibility Concerns**
Given the reproducibility score of 2, we wish to emphasize that all base models and datasets used in this study are publicly available. We also plan to release the training code upon the paper's publication, ensuring our results can be replicated and extended by others.

**Inspiration from Backpack Language Models**
The noted similarity of our method to backpack language models is intriguing, although it was not a direct inspiration for our approach. We appreciate this observation and consider it a valuable perspective that enriches the context of our work.

**Initialization Strategy in Parameterization**
Our method and Prefix-Tuning share the use of an up-projection linear layer. The primary distinction lies in our initialization strategy; we leverage samples from the embedding layer for initialization, as opposed to Prefix-Tuning’s approach of random initialization. This key differentiation, which we believe significantly impacts the effectiveness of our method, will be more clearly articulated in the camera-ready version of our manuscript.

**Performance Improvement with Minimal Prompt Tokens**
The observed performance gap on large datasets is a natural consequence of tuning only a minuscule fraction (0.00008) of the total parameters. This is consistent with the correlation between the number of prompts and the performance gap with full fine-tuning, as discussed in ["The Power of Scale for Parameter-Efficient Prompt Tuning"](https://aclanthology.org/2021.emnlp-main.243) (Lester et al., EMNLP 2021). Furthermore, we believe that the performance gap narrows in larger models, as explored in ["Intrinsic Dimensionality Explains the Effectiveness of Language Model Fine-Tuning"](https://aclanthology.org/2021.acl-long.568) (Aghajanyan et al., ACL-IJCNLP 2021). Despite this performance gap, it's crucial to recognize the inherent advantages of prompt tuning, not only as the most parameter-efficient among PEFT methods but also for its potential to enhance research in areas like adversarial attacks and hard prompt tuning, as shown in ["Hard Prompts Made Easy: Gradient-Based Discrete Optimization for Prompt Tuning and Discovery"](https://openreview.net/forum?id=VOstHxDdsN) (Wen et al., NeurIPS 2023).

**Reparameterization and Weight Decay**
Addressing the effect of weight decay in our reparameterization approach, we clarify that beyond mitigating the negative impacts of weight decay, our strategy allows for the learning of adjustments (\(\Delta\) vector) with a reduced norm. This leads to minimal alterations from the original initialization.

We are hopeful that these clarifications and planned revisions will adequately address your concerns and significantly improve the manuscript. We thank you again for your constructive feedback and look forward to making the necessary enhancements.
