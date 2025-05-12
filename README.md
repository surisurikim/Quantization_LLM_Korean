# Practical Quantization of Open LLMs

<div align="center">
<a href="https://pseudo-lab.com"><img src="https://img.shields.io/badge/PseudoLab-S10-3776AB" alt="PseudoLab"/></a>
<a href="https://discord.gg/EPurkHVtp2"><img src="https://img.shields.io/badge/Discord-BF40BF" alt="Discord Community"/></a>
</div>

## 📋 프로젝트 개요

본 프로젝트는 오픈소스 대규모 언어 모델(LLM)의 양자화(Quantization) 기법을 비교 분석하고, 특히 양자화가 한국어와 영어 성능에 미치는 차별적 영향을 연구합니다. 다양한 양자화 라이브러리를 활용하여 모델 경량화를 실험하고, 언어별 성능 저하의 패턴을 파악하여 한국어에 최적화된 양자화 방안을 모색합니다.

### 핵심 가설
> **양자화 후 한국어 성능 저하가 영어보다 더 클 것이다.**

## 🎯 연구 목표

1. 다양한 오픈소스 LLM 모델의 양자화 전후 성능 비교
2. 주요 양자화 라이브러리(bitsandbytes, AWQ, GPTQ, GGUF)의 특성 분석
3. 양자화가 한국어와 영어 성능에 미치는 차별적 영향 측정
4. (후속 과제) 한국어 성능 저하의 원인 규명 및 최소화 방안 제시

## 🧪 연구 방법론

### 1단계: 모델 및 라이브러리 선정
- **대상 모델**: Qwen3, Qwen2.5, Llama3.2
- **양자화 라이브러리**: 
  - bitsandbytes (8-bit, 4-bit)
  - AutoAWQ
  - GPTQ
  - GGUF (llama.cpp)

### 2단계: 라이브러리 분석 및 정리
- 각 라이브러리의 작동 원리, 알고리즘적 특성 분석
- 구현 방식과 최적화 전략 비교
- 지원하는 비트 수준과 양자화 유형 정리

### 3단계: 양자화 구현 및 성능 평가
- 모델별, 라이브러리별 양자화 실행
- 평가 메트릭:
  - **영어**: MMLU, GSM8K, HumanEval 등 표준 벤치마크
  - **한국어**: KLUE, KoBEST, 자체 제작 평가셋

### 4단계: 결과 분석 및 후속 연구
- 언어별 성능 차이 패턴 분석
- 토크나이저 분석과 양자화 관계 연구
- 한국어에 최적화된 양자화 방안 제안

## 📊 예상 결과물

1. 다양한 양자화 라이브러리 비교 분석 보고서 (기술 블로깅)
   - https://smartest-suri.tistory.com/
2. 한국어와 영어 성능 차이 분석 결과
3. 양자화된 모델들의 추론 속도, 메모리 사용량 비교 자료

## 📚 참고 자료

- [Han, Song. TinyML and Efficient Deep Learning](https://hanlab.mit.edu/courses/2024-fall-65940)
- [bitsandbytes: 8-bit Methods for Efficient Deep Learning](https://github.com/TimDettmers/bitsandbytes)
- [AutoAWQ: Automatic Activation-aware Weight Quantization](https://github.com/casper-hansen/AutoAWQ)
- [GPTQ: Accurate Post-training Quantization for GPT Models](https://github.com/IST-DASLab/gptq)
- [llama.cpp: Inference of LLaMA model in pure C/C++](https://github.com/ggerganov/llama.cpp)


## 👨‍💻 연구자 정보

- **김슬** | [GitHub](https://github.com/yourusername) | [LinkedIn](https://linkedin.com/in/yourprofile)
- 가짜연구소 시즌 10 [EfficientML](https://github.com/Pseudo-Lab/EfficientML) 멤버 
