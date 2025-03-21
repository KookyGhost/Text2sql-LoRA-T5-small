# Text2sql-LoRA-T5-small
Finetune a t5-small model for text2sql generation using LoRA

# Model Performance
Rogue: 0.928

# Reference
Inspired by https://gist.github.com/mkeywood1/9e8411aef44cf18009aa3e4776501c08, who was inspired by https://huggingface.co/cssupport/t5-small-awesome-text-to-sql


Different from the full fine-tuning approaches, this is an attempt to train a small size LoRA adpater, which appears to be as good as if not better than the fully finetuned model (Rogue 0.928 vs 0.923).
