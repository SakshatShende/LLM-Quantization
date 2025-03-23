#  LLaMA 3B Quantization Benchmark

**Hardware**: RTX 3090 (24 GB VRAM)  
**Dataset**: 5% of WikiText2 (for perplexity evaluation)  
**Notebook**: [Quantization.ipynb](https://jpchpdot0vpybi-8888.proxy.runpod.net/lab/tree/workspace/quantization%281%29.ipynb)

| Model | Perplexity | Inference Time (s)  | Model Size  | Peak VRAM Usage  |
|-------|---------------|----------------------|---------------|--------------------|
|  **Base (FP16)** | `14.99` | `1.84s` | `5.98 GB` | `12,283 MB` |
|  **GPTQ (4-bit)** | `19.19` | `11.5s` | `0.73 GB` | `2,380 MB` |
|  **AWQ (bfloat16)** | `15.93` | `2.89s` | `0.73 GB` | `2,242 MB` |

---

### ⏱️ Training  Time
- **GPTQ Quantization**: ~10 mins  
- **AWQ Quantization**: ~5 mins  

 Results computed using LLaMA 3B on a rented RunPod instance.

---
![Graph(15)](https://github.com/user-attachments/assets/201dda68-0070-4a72-a83e-d6932e83dc4e)
![Graph(16)](https://github.com/user-attachments/assets/61ba7dc4-ce83-4b2b-bc92-ebb6d6047902)
![Graph(17)](https://github.com/user-attachments/assets/5ea550ef-45a6-4277-8112-de4d4a80a5f1)
![Graph(14)](https://github.com/user-attachments/assets/d9e5c00d-8a7f-4fc5-81c7-ad9fa68421e9)
