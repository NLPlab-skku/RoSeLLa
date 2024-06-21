# NLPLAB_sLM
# 한국어 기반 소형 언어 모델(sLM)

SKKU-NLPLAB-sLM은 NLPLAB에서 구축한 [NLPLAB sLM 데이터셋](https://github.com/NLPlab-skku/DATA/tree/main/sLM)을 기반으로 학습한 한국어 소형 언어 모델입니다.<br/>
[🤗42dot/42dot_LLM-PLM-1.3B](https://huggingface.co/42dot/42dot_LLM-PLM-1.3B)을 기반으로 instruction tuning 된 모델입니다.


## sLM.v0
NLPLAB sLM 데이터셋을 instruction tuning 한 모델입니다.<br/>
- Repo: [🤗SKKU-NLPLAB-sLM-v0](https://huggingface.co/NLPlab-skku/42dot_v0) <br/>

|데이터셋|개수|
|------|---|
|**CoT**|77,200|
|**Dolly**|6,642|
|**EverythingLM**|991|
|**Law**|13,702|
|**Number**|9,580|

## sLM.v1
NLPLAB sLM 데이터셋을 2차 가공하여 instruction tuning 한 모델입니다.<br/>
- Repo: [🤗SKKU-NLPLAB-sLM-v1](https://huggingface.co/NLPlab-skku/42dot_v1) <br/>

v0의 데이터 셋의 일부를 gpt-4o를 통하여 필터링하였습니다. <br/>
추후에 모든 데이터에 대해서 필터링 작업을 진행할 예정입니다. <br/>


