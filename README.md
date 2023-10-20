# Low Rank Adaptation

Implementing LoRA paper on a simple network for classifing a mnist

LoRA pros:
1. Decrese size of fine tuned model
2. Decrese letancy of fine tuning a model
3. Apility to switch between fine tuned models without needing to load the entire parametes each time

Code Steps:
1. Trained a big network with ~ 900K parameters to classifiy mnist
2. Built a LoRA Layer according to LoRA Paper
3. Replaced each dense layer with a LoRA Layer
4. The original parameters of the networks has been frozen
5. fine tuned the lora_model on images with label 2