# (Session 2) Microsoft Build - AI Odyssey

AI Odyssey
- 통과하면 경품주고
- 링크드인 배치줌

https://www.microsoft.com/ko-kr/AIOdyssey/

6월 25일까지 하면 됨

레벨1은 기본적인 내용(4가지)

금일 1, 3 주제를 진행
- 1. OpenAI
- 3. Vision

MS Azure Cognitive Services
- Vision등도 있다

> Azure AI
> 1. AI가 자동으로 Model을 만들어줌
>    * 데이터 있으면 자동으로 리스트업 해줌
>    * 모중고 사이트(KB)에서 사용하고 있음
> 2. Responsible AI Tooling
>    * 비즈니스에 알맞지 않는 것들을 빼줌


Foundation model
- 어떤 모델을 갈아넣을수 있게 있음
- Phi, Llama등


OpenAI에서 각 모델별로 가격이 따로 있음
주로 Azure에서 사용

## 시작
Azure에서
1. 리소스 그룹을 생성
2. 만들기를 눌러 만듬
3. 마켓플레이스(인프라 오픈마켓)
4. openai 검색 > azure openai
5. 사용량이 없으면 에러가 뜸
6. Region 선택 > 신규 센터에 여유가 있다
7. 이름은 유니크한 이름으로 지어야 한다.
8. 2~3분 정도 올라오는데 시간이 걸림
9. 키 및 엔드포인트에서 키랑 엔드포인트를 통해 접속을 할 수 있음(키는 두개중 하나만 있으면 됌)
10. 개요로 이동 > Azure OpenAI Studio로 이동
11. 왼쪽에서 모델을 선택
12. 모델을 검색하고 사용하는게 좋다. 이미지는 dall-e를 사용
    > turbo가 뒤에 붙어 있으면 성능이 잘나옴
    > 이왕이면 최신버전 쓰는게 좋음
    > 32k일 경우 token수를 거기까지 쓸수 있음
    > tts 모델은 whisper가 뛰어남
    > 3.5와 4의 가격은 10배 차이남
13. 배포를 누르면 모델 배포를 할 수 있음
14. 분당 사용한 토큰은 1k = 한글 1K자 -> 300K로 늘릴 수 있음
15. 만들기를 누르면 모델을 배포함


GPT 언어모델
- 오픈소스도 있고 클로즈 소스도 제공
- Llama3 : 오픈소스
- Phi3 : 오픈소스

GPT가 다는 아니다

Token
- OpenAI Tokenizer
- "I Love you"
- 의미 단위로 처리하는게 Token이다

한글은 토큰이 여러개다
- 한글은 많은 토큰을 소모
- gpt4-o는 1.7배만 쓴다
- azure openai에서만 사용할 수 있다.

Temperature
0 ~ 1사이
0은 언어모델에 있는 값만 가지고 대답
1은 창의적 극대화
보고서는 0.3

OCR, Image Analysis등 있음










