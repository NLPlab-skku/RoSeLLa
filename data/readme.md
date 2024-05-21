# sLM 데이터셋

NLPLAB에서 구축한 sLM 학습을 위한 Chain-of-Thought 기반의 데이터셋입니다.


## 구축내용
|제목|내용|위치|
|------|---|---|
|**CoT**|KAIST에서 발표한 [CoT-Collection](https://github.com/kaistAI/CoT-Collection)의 한국어 버전 데이터셋|./COT.jsonl|
|**Dolly**|Instruction Tuning을 위해 제작된 [Databricks-dolly-15k 데이터셋](https://huggingface.co/datasets/databricks/databricks-dolly-15k)을 한국어로 번역하고 ChatGPT API를 통해 rationale를 생성하여 만든 데이터셋|./dolly.jsonl|
|**EverythingLM**|Instruction Tuning을 위해 제작된 [EverythingLM V2 데이터셋](https://huggingface.co/datasets/totally-not-an-llm/EverythingLM-data-V2)을 한국어로 번역하고 ChatGPT API를 통해 rationale를 생성하여 만든 데이터셋|./every.jsonl|
|**Law**|AI허브의 [문서 요약 텍스트 데이터셋](https://aihub.or.kr/aihubdata/data/view.do?currMenu=&topMenu=&aihubDataSe=data&dataSetSn=97)을 기반으로 ChatGPT API를 통해 rationale를 생성하여 만든 법률 요약 데이터셋|./law.jsonl|
|**Number**|AI허브의 [숫자연산 기계독해 데이터셋](https://www.aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&dataSetSn=71568)을 기반으로 ChatGPT API를 통해 rationale를 생성하여 만든 숫자연산 데이터셋|./number.jsonl|

## 데이터 통계
<table class="tg">
<thead>
  <tr>
    <th class="tg-c3ow"></th>
    <th class="tg-c3ow">CoT</th>
    <th class="tg-c3ow">Dolly</th>
    <th class="tg-c3ow">EverythingLM</th>
    <th class="tg-c3ow">Law</th>
    <th class="tg-c3ow">Number</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-c3ow">Train</td>
    <td class="tg-c3ow">77,200</td>
    <td class="tg-c3ow">6,642</td>
    <td class="tg-c3ow">991</td>
    <td class="tg-c3ow">13,702</td>
    <td class="tg-c3ow">9,580</td>
  </tr>
</tbody>
</table>
