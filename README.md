# Text2sql-LoRA-T5-small
The Python notebooks document step by step process of finetuning t5-small model for text2sql generation using a LoRA adapter.

# Model Performance
Rogue: 0.928

# Download LoRA Adapter File
git clone https://huggingface.co/KookyGhost/txt2sql-LoRA-adapter-t5-small

# Download LoRA + Base Model File 
git clone https://huggingface.co/KookyGhost/txt2sql-LoRA-merged-t5-small
This is a merged model that can be used directly swithout the need to manually apply the adapter.

# Reference
Inspired by https://gist.github.com/mkeywood1/9e8411aef44cf18009aa3e4776501c08, who was inspired by https://huggingface.co/cssupport/t5-small-awesome-text-to-sql, where the former is a recreation of the latter, by fully finetuning the base t5-small model.

# Summary
Different from the full fine-tuning approach, this is an attempt to train a small size LoRA adpater, which appears to be as good as if not better than the fully finetuned model (Rogue score: 0.928 vs 0.923) on the test set. The LoRA approach significantly reduces the number of trainable parameters, from 60,506,624 (100%) to 294,912 (0.49%), making fine-tuning faster, more memory-efficient, and computationally cheaper, without sacrificing the model performance.
