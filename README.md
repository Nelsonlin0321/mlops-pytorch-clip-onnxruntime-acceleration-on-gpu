
# Inference PyTorch CLIP Model with ONNX Runtime on CPU


## Introduction

This tutorial will introducee to how convert HuggingFace [CLIP Model](https://huggingface.co/openai/clip-vit-base-patch32) to ONNX, and inference it for high performance using ONNX Runtime On GPU. See the below comparisons between native pytorch and onnx on gpu inference, we notice that ONNX can much accelebrate the inference and it has been one of best choice for deployment of our LLM models for cost saving and more efficiency.

And, now we try to convert CLIP to ONNX and inference it using ONNX Runtime !

Please follow the tutorial colab to try it out:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1__9FlKNHsHNXcaN095z1-IMhPjgeeZvV)

## Conclusion:
Using ONNX Runtime is 3.51 × Faster than using Pytorch on GPU infernece.

CLIP only takes 9 ms inferencing an images whereas pytorch takes 41 ms in average. 
<img src="Speed-up.png"></img>


## Referene:
Medium post about accelerating other Hugging Face models:

https://medium.com/microsoftazure/accelerate-your-nlp-pipelines-using-hugging-face-transformers-and-onnx-runtime-2443578f4333

<img src='https://miro.medium.com/v2/resize:fit:720/format:webp/1*4GREvqUWnFU9VXuNk2HEFQ.png'></img>



