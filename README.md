# dont-stop-pretraining
Implementing of the paper "Don’t Stop Pretraining: Adapt Language Models to Domains and Tasks" (ACL 2020) in fast.ai and Huggingface transformers library.

This is a minimal version that works only for a LM trained using MLM task (BERT, ROBERTA, etc). To modify it to a regressive model is trivial. You just need to modify the pre-processing for the pre-training task.

## TODOs:

1. Use larger batch size during fine-tuning LM as detailed in the paper. (Can be done with gradient accumulation with [TrainingArguments](https://huggingface.co/transformers/main_classes/trainer.html#transformers.TrainingArguments) in HuggingFace library).
2. Use a smaller learning rate following the paper.
3. Try pre-training more epochs!
4. Try graduate unfreezing layers during training classifier.
5. Try a regressive LM (should be easier but the performance may not be as good due to lack of bi-directional encoding).
