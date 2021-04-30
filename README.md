# dont-stop-pretraining
Implementing of the paper "Don’t Stop Pretraining: Adapt Language Models to Domains and Tasks" (ACL 2020) in fast.ai and Huggingface transformers library.

This is a minimal version that works only for a LM trained using MLM task (BERT, ROBERTA, etc). To modify it to a regressive model is trivial. You just need to modify the pre-processing for the pre-training task.
