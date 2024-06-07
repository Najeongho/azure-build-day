#1. Azure Prompt Flow 가장 쉬운 RAG

> 경량화된 온디바이스 LLM
> * Google Gemma
> * MS Phi

> 크롤링된 데이터
> * Common Crawl에서 가져옴

> 한계점
> * Hallucination
> * 최신 데이터 반영 안함
> * 모른다고 하지 않음
> * Token 수 제한

gpt-4o의 경우, 2023 Oct 정보를 학습함

최신 데이터를 사용할 수 있는 방법
1. Fine Tuneing
> * 새로운 모델을 만듬
> * 하면 좋은데 학습에 대한 시간과 리소스가 듬
2. Prompt Engineering
> * 모델이 잘 결과를 낼 수 있도록 엔지니어링 함

Prompt : 인공지능이 무언가를 할 수 있도록 하는 것임
> * 생성형 인공지능이 더 나은 결과물을 만들어 낼 수 있도록 prompt 설계
> * 프로그래밍 기술 활용, 외부데이터/기술 연동

RAG(Retrieval Augmentated Generation, 증강 생성 검색)
> * 중간에 데이터베이스에서 사용자 질문에 유사한 질문을 검색
> * RAG가 중요한 기술중 하나임

RAG는 Meta에서 2020년 경에 만든 기술임

MS에서는 RAG가 Core라는 것을 언급

RAG는 다양한 자료로 연결 가능
> * PDF등
> * Keyword 기반으로는 옛날 방식임
> * 유연하게 검색할 수 있는 기법
> * * Embedding

Embedding Model은 Deep Learning 기법
> 사람의 문장 및 단어를 숫자로 변환하는게 Embedding model
> 숫자는 Vector에 저장

Vector는 Cosine Similarity를 통해 가까운 것을 통해 유사도등 숫자를 나타낼 수 있음

2개 모델이 필요함
1. Embedding
2. ?

정보 가져오는 순서
LOAD -> Spilt -> Embedding -> Store

Question이 들어오게 되면 Retrieval을 하게 된다(Vector에서)
-> 언어모델 한계점을 극복할 수 있다. (할루시네이션 등)

Vector Storage
- Pinecone
- FAISS (Facebook)
- Weaviate
- Chroma

RAG
- MS Semantic Kernel
- > Prompt flow (testing -> Deploying)
- LangChain

벡터를 저장하는 방법을 제공
> 리소스는 내일까지 사용 가능

https://bit.ly/2024buildkr































