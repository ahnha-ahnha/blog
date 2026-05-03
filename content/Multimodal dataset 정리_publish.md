# Fine-tuning
1. [https://huggingface.co/datasets/EchoSafe-MLLM/MM-SafetyBench-plus-plus](https://huggingface.co/datasets/EchoSafe-MLLM/MM-SafetyBench-plus-plus "https://huggingface.co/datasets/echosafe-mllm/mm-safetybench-plus-plus")
    1. 시각적으로나 텍스트적으로는 유사해 보이지만 안전 의도는 크게 다른 시나리오 간의 미묘한 문맥적 차이를 모델이 구별하도록 요구
    2. 2,844, cc-by-4.0 (저작자 표시 사용가능)
    3. - Illegal Activity - Hate Speech - (and others)
2. [https://huggingface.co/datasets/AI-Safeguard/Img_VLM](https://huggingface.co/datasets/AI-Safeguard/Img_VLM "https://huggingface.co/datasets/ai-safeguard/img_vlm")
    1. 277GB 생성 데이터, 데이터 까서 보고 안전하면 Safe 생성 데이터로 사용가능, apache-2.0
3. [https://huggingface.co/datasets/AI-Safeguard/Ivy-Fake](https://huggingface.co/datasets/AI-Safeguard/Ivy-Fake "https://huggingface.co/datasets/ai-safeguard/ivy-fake")
    1. - 이미지와 비디오에서 합성 아티팩트를 식별을 위한 데이터셋, Safe video, image로 사용가능
    2. 15만 개 이상의 학습 샘플(이미지 + 비디오) - 18,700개의 평가 샘플
4.  [https://huggingface.co/datasets/jayzou3773/SafeFlowBench](https://huggingface.co/datasets/jayzou3773/SafeFlowBench "https://huggingface.co/datasets/jayzou3773/safeflowbench")
    1. 적대적이고 기만적인 멀티모달 시나리오에서 LLM/VLM 기반 에이전트의 견고성, 보안 및 결정 무결성을 평가하도록 설계된 구조화된 벤치마크
        1. - **웹페이지** , **앱** , **운영체제** 환경 전반에 걸친 **332가지 시나리오**
        2. 다양한 **위협 분류 체계** : 시각적 기만, 콘텐츠/텍스트 위조, 상호작용 함정, 실행 수준 공격 등.
        3. 재현성 및 판단 일관성을 위한 **명확한 평가 원칙** 과 함께 풍부한 멀티모달 입력(예: 스크린샷, 프롬프트)을 활용합니다.
        4. MIT license
5. [https://huggingface.co/datasets/thu-coai/MIR-SafetyBench](https://huggingface.co/datasets/thu-coai/MIR-SafetyBench "https://huggingface.co/datasets/thu-coai/mir-safetybench")
    1. 다중 이미지 관계(MIR) 기반 보안 공격에 대한 다중 모달 대규모 언어 모델(MLLM) 평가를 위한 포괄적인 평가 프레임워크
    2. 6가지 안전 범주와 9가지 관계 유형에 걸쳐 다중 이미지 관계 공격을 통해 MLLM의 안전성을 평가합니다.
        1. **안전 등급:** 혐오 발언, 폭행, 자해, 불법 활동, 괴롭힘, 은둔
        2. **관계 유형:** 유추, 인과관계, 상호보완성, 분해, 관련성, 공간 임베딩, 공간적 병치, 시간적 연속성, 시간 도약
	3. MIT license
6. https://huggingface.co/datasets/chadlzx/USB-SafeBench
	1. [USB: A Comprehensive and Unified Safety Evaluation Benchmark for Multimodal Large Language Models](https://arxiv.org/abs/2505.23793v1) 논문 데이터셋 
	2. 17,763 rows, apache 2.0
7. 
# Benchmark
1. [https://huggingface.co/datasets/PKU-Alignment/MM-SafetyBench](https://huggingface.co/datasets/PKU-Alignment/MM-SafetyBench "https://huggingface.co/datasets/pku-alignment/mm-safetybench")
    - 6,720, **cc-by-nc-4.0 (학습 사용불가)**
2. [https://huggingface.co/datasets/firaapril/child-safe-vlm-databaru/tree/main/images](https://huggingface.co/datasets/firaapril/child-safe-vlm-databaru/tree/main/images "https://huggingface.co/datasets/firaapril/child-safe-vlm-databaru/tree/main/images")
    1. 아동 괴롭힘 합성 이미지, 105개
    2. no license
3.  [https://huggingface.co/datasets/ArthT/vlm-safety-circuits](https://huggingface.co/datasets/ArthT/vlm-safety-circuits "https://huggingface.co/datasets/artht/vlm-safety-circuits")
    1. **각 항목에는 38개의 안전 범주** 에 걸쳐 유해/무해한 반사실적 상황 쌍이 포함되어 있으며, 50개의 JailbreakBench 스타일 프롬프트가 제공됩니다. 데이터 세트는 세 가지 유형의 반사실적 상황을 다룹니다.
        1. |Text counterfactual|226|Same image, harmful vs. benign text|
        2. |Image counterfactual|150|Same text, harmful vs. benign image|
        3. |Typographic attack|44|Harmful text embedded in image|
    2. 325? 420?, MIT
4. [https://huggingface.co/datasets/oneonlee/Meme-Safety-Bench](https://huggingface.co/datasets/oneonlee/Meme-Safety-Bench "https://huggingface.co/datasets/oneonlee/meme-safety-bench")
    1. MemeSafetyBench는 유해한 지침과 무해한 지침을 실제 밈 이미지와 짝지어 제공하는 50,430개의 인스턴스로 구성된 종합적인 벤치마크 데이터셋
    2. 46,599개의 유해 샘플(92.4%)  - 3,831개의 무해한 샘플(7.6%)
    3. `MemeSafetyBench-Mini`총 390개의 샘플
        1. 유해 샘플 330개(92.4%) (- 12가지 유해 물질 범주당 30개 샘플)
        2. 무해한 샘플 30개(7.6%)
    4. no-license
5. [https://huggingface.co/datasets/kzhou35/mssbench](https://huggingface.co/datasets/kzhou35/mssbench "https://huggingface.co/datasets/kzhou35/mssbench")
    1. [https://github.com/eric-ai-lab/MSSBench](https://github.com/eric-ai-lab/MSSBench "https://github.com/eric-ai-lab/mssbench")
    2. json 파일에 text가 있음. 공간에 대한 상황설명이 safe 한지
    3. 724, MIT
6. [https://huggingface.co/datasets/sinwang/SIUO](https://huggingface.co/datasets/sinwang/SIUO "https://huggingface.co/datasets/sinwang/siuo") (원본)
    1. [https://huggingface.co/datasets/oneonlee/SIUO](https://huggingface.co/datasets/oneonlee/SIUO "https://huggingface.co/datasets/oneonlee/siuo") (사용하기 좋게)
    2. SIUO (Safe-Input Unsafe-Output),  json 파일에 text가 있음
        1. `siuo_gen`: 안전 경고 및 참조 답변을 포함한 생성 작업 구성 (167항)
        2. `siuo_mcqa`객관식 QA 과제 구성 (선택지 및 정답 포함) (167항)
    3. 334, no-license
7. [https://github.com/paul-rottger/msts-multimodal-safety/tree/main/data](https://github.com/paul-rottger/msts-multimodal-safety/tree/main/data "https://github.com/paul-rottger/msts-multimodal-safety/tree/main/data")
    1. safe Imgae + safe text => unsafe result, 영어, 한국어 다 있음
    2. 각 400개  cc-by-4.0
8. [https://github.com/apple/ml-vlsu](https://github.com/apple/ml-vlsu "https://github.com/apple/ml-vlsu")
    1. **8,187** image-text pairs with **human annotations** across three dimensions: image-only, text-only, and joint safety
    2. **17 severity combinations** spanning the complete safety spectrum
    3. **15 taxonomy categories** for comprehensive harm coverag
    4. cc-by-nc-nd (학습 사용불가)
9. [https://github.com/Jarviswang94/MMSafetyAwareness](https://github.com/Jarviswang94/MMSafetyAwareness "https://github.com/jarviswang94/mmsafetyawareness")
    1. 29가지 안전 시나리오와 1,500개의 엄선된 이미지-프롬프트 쌍을 통해 다중 모드 안전 인식 모델을 평가하도록 설계된 최초의 포괄적인 다중 모드 안전 인식 벤치마크
    2. (Unsafe subset): Safe Image + Safe Text -> Unsafe
    3. (Over-Safety subset): Image, Text 각각은 Unsafe로 느껴질 수 있음 -> Image+Text 맥락에서 Safe
    4. no-license
10. https://huggingface.co/datasets/Advait-s06/safety-image-pairs
	1. 유사한 맥락의 사진을 '안전(Safe)'과 '위험(Unsafe)'으로 짝을 지어 제공
	2. 비슷한 구도나 사물이 포함되어 있지만, 결정적인 상황(Context)에 따라 레이블이 갈리는 쌍
	3. 185 pairs, 검증용, no-license
11. [https://huggingface.co/datasets/yizhilsy/Toy_SafetyBench_jailbreak_rq](https://huggingface.co/datasets/yizhilsy/Toy_SafetyBench_jailbreak_rq)
	1. 소규모 Jailbreak 4000 rows, no-license
12. https://huggingface.co/datasets/albertklorer/safedocs
	1. OCR 기반 가드레일 170,000 rows, no-license
13. https://huggingface.co/datasets/PahaII/vllm_safety_evaluation
	1. 소규모 Adversarial Jailbreak OOD testset 1,991 rows, no-license
14. https://huggingface.co/datasets/tyodd/SafeEditBench
	1. 이미지 편집 결과물에 대해 자유방임부터 극단적 통제까지 5단계 정책(L1~L5)에 맞춰 VLM이 유연하게 유해성을 판단할 수 있는지 측정하는 **'정책 적응형(Policy-Adaptive)' 멀티모달 가드레일 평가 데이터셋**
	2. 601 rows, cc-by-4.0
15. https://huggingface.co/datasets/Lenkashell/safe_harassment_image_captions
	1. 대인관계 괴롭힘 소규모 image-caption pair 데이터셋 100 rows, no-license 
16. https://huggingface.co/datasets/HappyCorpse/SafeMT
	1. Multi-turn Dialogue Benchmark 
	2. 유해 질의 2000개 대화 데이터 8000개 총 10,000 rows, cc-by-nc-4.0
17. https://huggingface.co/datasets/Machlovi/SafeorNotSafe
	1. Safe/Not Safe 
18. https://huggingface.co/datasets/oceanikkaaa/safety-dataset-8.2
19. 
# RLHF/DPO
1. [https://huggingface.co/datasets/PKU-Alignment/PKU-SafeRLHF-V](https://huggingface.co/datasets/PKU-Alignment/PKU-SafeRLHF-V "https://huggingface.co/datasets/pku-alignment/pku-saferlhf-v")
    1. 멀티모달 RL용 데이터셋, 9개의 주요 안전 영역, 텍스트 정보와 이미지를 포함한 다양한 콘텐츠로 구성되어 있으며, 유해하거나 부적절한 콘텐츠를 탐지하는 데 도움이 되도록 특정 범주로 분류
    2. 30,414, **cc-by-nc-4.0 (학습 사용불가)**
    3. 1. Threats to National and Public Security, 2. Health and Safety Risks, 3. Physical and Psychological Harm, 4. Privacy and Consent Violations, 5. Discrimination and Harassment, 6. Unethical Betrayal and Deceptive Behavior, 7. False Information and Sensitive Information, 8. Disturbing or Unsettling Content, 9. Sexually Explicit and Inappropriate Content
2. https://huggingface.co/datasets/saferlhf-v/BeaverTails-V
	1. 이 데이터셋의 가장 큰 특징은 단순히 '유해하다/아니오'만 가리는 게 아니라, **두 가지 답변 중 무엇이 더 나은지(Preference)**를 비교
		- **데이터 구조:** `이미지 + 질문` 하나에 대해 **두 개의 서로 다른 VLM 답변**이 붙어 있음
		- **레이블링:**  어느 답변이 더 **도움이 되는가**(Helpful)?
		    - 어느 답변이 더 **안전한가**(Safer)?
		    - 각 답변의 **무해함(Harmless) 점수**와 **도움(Helpful) 점수**가 수치화
	2. 30,414 rows, cc-by-nc-4.0
	3. Taxonomy : 국가안보 / 건강 및 안전 / 물리심리적 가해 / 개인정보 / 차별 및 괴롭힘 / 비윤리적 행위 / 허위 정보 / 혐오 콘텐츠 / 성적 콘텐츠
3. https://huggingface.co/datasets/XuankunRong/SafeTag-VL-3K
	1. 멀티모달 모델(VLM)이 단순히 유해한 것을 "안다"를 넘어, "왜 유해한지 논리적으로 추론"하게 만들기 위해 설계된 고도화된 데이터셋
	2. 멀티모달 RL용 데이터셋, 명시적인 시각적, 텍스트적, 그리고 결합된 안전 태그를 특징
	3. 3,293  rows, 잘못된 태그 보임. no-license
4. https://huggingface.co/datasets/Holly301/Think-in-Safety
	1. TiS는 `<think>` 태그 안에 모델이 이 요청을 왜 안전하다고 혹은 유해하다고 판단했는지에 대한 '추론 과정'을 포함
	2. 4396 rows, apache 2.0

# Image
1. https://huggingface.co/datasets/Mitsua/safe-commons-pd-3m
	1. **규모:** 약 **304만 개(3.04M)**의 이미지-텍스트 쌍 - Safe 이미지
	2. CC BY-SA 4.0
2. 
# Insight
1. SafeWatch
- Video guardrail 

- [ ] https://huggingface.co/openai/privacy-filter