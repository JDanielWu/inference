.. _models_llm_qwq-32b:

========================================
QwQ-32B
========================================

- **Context Length:** 131072
- **Model Name:** QwQ-32B
- **Languages:** en, zh
- **Abilities:** chat, reasoning, tools
- **Description:** QwQ is the reasoning model of the Qwen series. Compared with conventional instruction-tuned models, QwQ, which is capable of thinking and reasoning, can achieve significantly enhanced performance in downstream tasks, especially hard problems. QwQ-32B is the medium-sized reasoning model, which is capable of achieving competitive performance against state-of-the-art reasoning models, e.g., DeepSeek-R1, o1-mini.

Specifications
^^^^^^^^^^^^^^


Model Spec 1 (pytorch, 32 Billion)
++++++++++++++++++++++++++++++++++++++++

- **Model Format:** pytorch
- **Model Size (in billions):** 32
- **Quantizations:** none
- **Engines**: vLLM, Transformers, SGLang
- **Model ID:** Qwen/QwQ-32B
- **Model Hubs**:  `Hugging Face <https://huggingface.co/Qwen/QwQ-32B>`__, `ModelScope <https://modelscope.cn/models/Qwen/QwQ-32B>`__

Execute the following command to launch the model, remember to replace ``${quantization}`` with your
chosen quantization method from the options listed above::

   xinference launch --model-engine ${engine} --model-name QwQ-32B --size-in-billions 32 --model-format pytorch --quantization ${quantization}


Model Spec 2 (awq, 32 Billion)
++++++++++++++++++++++++++++++++++++++++

- **Model Format:** awq
- **Model Size (in billions):** 32
- **Quantizations:** Int4
- **Engines**: vLLM, Transformers, SGLang
- **Model ID:** Qwen/QwQ-32B-AWQ
- **Model Hubs**:  `Hugging Face <https://huggingface.co/Qwen/QwQ-32B-AWQ>`__, `ModelScope <https://modelscope.cn/models/Qwen/QwQ-32B-AWQ>`__

Execute the following command to launch the model, remember to replace ``${quantization}`` with your
chosen quantization method from the options listed above::

   xinference launch --model-engine ${engine} --model-name QwQ-32B --size-in-billions 32 --model-format awq --quantization ${quantization}


Model Spec 3 (mlx, 32 Billion)
++++++++++++++++++++++++++++++++++++++++

- **Model Format:** mlx
- **Model Size (in billions):** 32
- **Quantizations:** 3bit, 4bit, 6bit, 8bit, bf16
- **Engines**: MLX
- **Model ID:** mlx-community/QwQ-32B-{quantization}
- **Model Hubs**:  `Hugging Face <https://huggingface.co/mlx-community/QwQ-32B-{quantization}>`__, `ModelScope <https://modelscope.cn/models/mlx-community/QwQ-32B-{quantization}>`__

Execute the following command to launch the model, remember to replace ``${quantization}`` with your
chosen quantization method from the options listed above::

   xinference launch --model-engine ${engine} --model-name QwQ-32B --size-in-billions 32 --model-format mlx --quantization ${quantization}


Model Spec 4 (ggufv2, 32 Billion)
++++++++++++++++++++++++++++++++++++++++

- **Model Format:** ggufv2
- **Model Size (in billions):** 32
- **Quantizations:** BF16, IQ4_NL, IQ4_XS, Q2_K, Q2_K_L, Q3_K_M, Q3_K_S, Q4_0, Q4_1, Q4_K_M, Q5_K_M, Q6_K, UD-IQ1_M, UD-IQ1_S, UD-IQ2_M, UD-IQ2_XXS, UD-IQ3_XXS, UD-Q2_K_XL, UD-Q3_K_XL, UD-Q4_K_XL, UD-Q5_K_XL, UD-Q6_K_XL, UD-Q8_K_XL, Q8_0
- **Engines**: vLLM, llama.cpp
- **Model ID:** unsloth/QwQ-32B-GGUF
- **Model Hubs**:  `Hugging Face <https://huggingface.co/unsloth/QwQ-32B-GGUF>`__, `ModelScope <https://modelscope.cn/models/unsloth/QwQ-32B-GGUF>`__

Execute the following command to launch the model, remember to replace ``${quantization}`` with your
chosen quantization method from the options listed above::

   xinference launch --model-engine ${engine} --model-name QwQ-32B --size-in-billions 32 --model-format ggufv2 --quantization ${quantization}

