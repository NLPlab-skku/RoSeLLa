# RoSeLLa
# 한국어 기반 소형 언어 모델(sLM)

RoSeLLa는 NLPLAB에서 구축한 [NLPLAB sLM 데이터셋](https://github.com/NLPlab-skku/DATA/tree/main/sLM)을 기반으로 학습한 한국어 소형 언어 모델입니다.<br/>
[🤗42dot/42dot_LLM-PLM-1.3B](https://huggingface.co/42dot/42dot_LLM-PLM-1.3B)을 기반으로 instruction tuning 된 모델입니다.


## RoSeLLa.v0
NLPLAB sLM 데이터셋을 instruction tuning 한 모델입니다.<br/>
- Repo: [🤗NLPlab-skku/Rosella_v0](https://huggingface.co/NLPlab-skku/RoSeLLa_v0) <br/>

|데이터셋|개수|
|------|---|
|**CoT**|77,200|
|**Dolly**|6,642|
|**EverythingLM**|991|
|**Law**|13,702|
|**Number**|9,580|

## RoSeLLa.v1
NLPLAB sLM 데이터셋을 2차 가공하여 instruction tuning 한 모델입니다.<br/>
- Repo: [🤗NLPlab-skku/Rosella_v1](https://huggingface.co/NLPlab-skku/RoSeLLa_v1) <br/>

v0의 데이터 셋의 일부를 gpt-4o를 통하여 필터링하였습니다. <br/>

## RoSeLLa.v2 (진행중)
기존 오픈소스 LLM을 활용하여 Pruning 및 Knowledge Distillation 기법을 적용한 경량화 모델입니다.
- Repo: (7~8월 중 공개 예정)

Base Model: Llama-3-3B, Qwen2.5-3B, Gemma-2B 등

**Pruning:** <br/>
1. 중요도가 낮은 attention/MLP weight 제거 (Magnitude-based & Head-wise pruning) <br/>
2. 중요도가 낮은 Layer 제거

**Knowledge Distillation:** 각 Base Model을 교사(teacher)로 설정하여 Hidden States, Logits, Final Output을 기반으로 Student 모델을 학습

기반 데이터 : [openwebtext](https://skylion007.github.io/OpenWebTextCorpus)

이후 전체 과정을 **반복적으로 수행**

목표: 모델 크기 및 추론 비용을 줄이면서도 기존 Instruction 능력 유지
