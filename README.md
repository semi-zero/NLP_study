**텐서플로우와 머신러닝으로 시작하는 자연어처리 공부 코드 모음** 



***공지: GPT2 모델 다운로드 링크**
```
wget https://github.com/NLP-kr/tensorflow-ml-nlp-tf2/releases/download/v1.0/gpt_ckpt.zip -O gpt_ckpt.zip
```


# NLPBOOK

텐서플로2와 머신러닝으로 시작하는 자연어처리(로지스틱회귀부터 BERT와 GPT2까지)  
<p align="center">
  <img src="main.png" width="450" height="500" /> 
</p>

## 소개 (Introduction)

책에 수록된 자연어 처리 예제들에 주석을 달아 공부용으로 게재


## 설치방법 (Environments)

해당 자연어처리 예제에 대한 다양한 개발 환경 지원을 위한 도커(Docker) 가이드 추가

향후 예제에 대한 실습 패키지 업데이트 변화에 대응하기 위해 도커 사용을 권장

## Jupyter Docker 실행 (권장)

Docker 환경 사용시 19.03 이후 버전을 사용

- `bash build_jupyter_cpu.sh` 또는 `bash build_jupyter_gpu.sh`를 실행하면 docker image을 생성
- `bash exec_jupyter_cpu.sh` 또는 `bash exec_jupyter_gpu.sh`를 실행하면 docker환경에서 jupyter가 실행
-  jupyter 실행 포트번호는 8889 이므로 해당 포트번호에 대해서 사용이 가능해야 함



- 아나콘다 파이썬 가상 환경 구성

```
conda create -n {사용할 환경 이름} python=3.6
conda activate {사용할 환경 이름} 
# source activate {사용할 환경 이름} 
pip install -r requirements.txt
```
<!--** 추가로 본 실습에서는 `tensorflow==2.2.0` 환경에서 작동-->


```
conda install python=3.6
```
<!-- #### GPU 사용 시 CUDA 설치 관련 -->

<!-- - GPU를 사용하는 경우에는 텐서플로우와 호환이 되는 CUDA Version을 맞춰 설치-->
<!-- - 현재 본 프로젝트는 `tensorflow==1.10` 버전에서 실행이 가능하도록 구현 및 테스트-->
<!-- - `tensorflow-gpu==1.10` 의 경우 `CUDA 9.0`을 설치-->

<!-- >> - `tensorflow-gpu>=1.13` 의 경우 `CUDA 10.0`을 설치 -->
<!-- >> - `tensorflow-gpu>=1.5,<=1.12` 의 경우 `CUDA 9.0`을 설치-->
<!-- >> - `tensorflow-gpu>=1.0,<=1.4` 의 경우 `CUDA 8.0`을 설치-->

## 목차 (Table of Contents)

**준비 단계** - 자연어 처리에 대한 배경과 개발에 대한 준비


1. [자연어 처리 개발 준비](./1.NLP_PREP)
2. [자연어 처리 개요](./2.NLP_INTRO)

**자연어 처리 기본** - 자연어 처리 기본적인 모델 연습

3. [텍스트 분류](./3.TEXT_CLASSIFICATION)
4. [텍스트 유사도](./4.TEXT_SIM)

**자연어 처리 심화** - 챗봇 모델을 통한 심화된 자연어 처리

5. [챗봇 만들기](./5.CHATBOT)
6. [미세 조정 학습](./6.PRETRAIN_METHOD)

## Colab 실습

Colab 실습은 6장에 한하여 별도 저장소를 공개

- [저장소 링크](https://github.com/NLP-kr/tensorflow-ml-nlp-tf2-colab)




## 저작권
ChangWookJun / @changwookjun (changwookjun@gmail.com)  
Taekyoon  / @taekyoon (tgchoi03@gmail.com)  
JungHyun Cho  / @JungHyunCho (reniew2@gmail.com)  
Ryan S. Shin / @aiscientist (sungjin7127@gmail.com)
