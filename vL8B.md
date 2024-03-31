Thank you for the constructive review and the appreciation of our work's strengths, especially regarding the novelty of SuperPos-Prompt and our analysis on dropout. Your feedback is invaluable in guiding the improvement of our manuscript.

**Response to Weaknesses**

**Token Interpretability Analysis**: We acknowledge the importance of token interpretability in prompt tuning. Our future work aims to delve deeper into this aspect, potentially integrating methods like those suggested in [Hard Prompts Made Easy: Gradient-Based Discrete Optimization for Prompt Tuning and Discovery](https://openreview.net/forum?id=VOstHxDdsN) (Wen et al., NeurIPS 2023), which could provide a structured approach to enhancing interpretability.

**Significance of Removing Dropout**: Our findings indicate that removing dropout does not universally enhance prompt tuning performance. It's widely accepted to employ dropout during fine-tuning; our results suggest this might not always be beneficial and could potentially hinder performance. This observation aims to contribute to a nuanced understanding of dropout's role in the specific context of prompt tuning.

**Response to Comments, Suggestions, And Typos**

**Consistency in Contribution Presentation and Model Terminology**: We appreciate your pointing out these inconsistencies. Ensuring clarity and uniformity throughout the manuscript is crucial, and we will revise these sections to reflect a consistent order of contributions and uniform terminology for the T5-v1.1-lm-adapt model in our final version.

**Impact of Dropout on Model Performance**: Regarding the dropout's relevance, our initial approach adhered to conventional fine-tuning practices, including re-enabling dropout as suggested by Google for T5 models. However, our empirical findings specifically with the T5-v1.1-lm-adapt model revealed a substantial performance degradation when dropout was applied during prompt tuning, exceeding a 7.0 score loss. This observation was significant enough to warrant mention in our paper, highlighting a potential model-specific impact of dropout on prompt tuning performance. While our resource constraints limited the scope of experimentation across various models, this insight into dropout's effect offers a compelling direction for future research to ascertain if similar trends are observable with other architectures.

**Reporting SuperPos-Prompt with Dropout**: The decision to focus on our most successful method without dropout was to highlight its performance advantages. However, including results with dropout for a direct comparison is valuable, and we will aim to add this analysis in our final revision. Exploring how dropout's impact varies across different base models is indeed an interesting avenue for future work, which we plan to pursue further.

Your feedback has been instrumental in highlighting areas for clarification and improvement. We are committed to addressing these points to enhance the soundness and contribution of our work. Thank you again for your thorough review.
