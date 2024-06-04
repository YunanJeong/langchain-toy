# langchain-toy

## 국룰 툴

- LangChain: LangChain은 다양한 언어 모델을 통합하여 하나의 플랫폼에서 사용할 수 있게 하고, 이를 통해 모델을 쉽게 비교하고 선택할 수 있도록 돕는 SDK
  - LLM 자체를 건드리는 툴은 아니고, LLM을 활용할 수 있게 도와주는 툴
  - JS, Python 가능한데 Python이 주류
  - 나머지 아래 기술되는 툴들도 전부 파이썬 라이브러리
  - 자체적으로 오픈소스 LLM 제공하진 않음
  - 오픈소스 LLM을 지원하는 다른 라이브러리와 연동 필요
  - OpenAI API는 LangChain 단독으로 직접 접근 가능
- Streamlit
  - 간단한 웹앱을 만들기 위한 파이썬 라이브러리. ChatGPT같은 웹페이지 화면 뚝-딱
  - 데이터 분야에서 빠르게 가시화하는 용도로 사용됨
  - 접속세션마다 파이썬 intepreter 연산이 실행되므로 사용자가 아주 많은 서비스엔 부적절
- Hugging Face Transformers: 다양한 사전 학습된 LLM을 제공하며, 이를 쉽게 사용할 수 있는 API와 도구를 제공. LangChain과 연동하여 사용하면 된다.

## 예시: Prometheus LangChain Agent

- 결국 LangChain으로 무슨 서비스를 만들거냐가 중요한데 Grafana없이 Prometheus로 자연어기반 쿼리 날리는 게 있다.
- [기존 시도](https://gist.github.com/jcanizalez/e089e3ab8eaf119f8ee622cfa364ed8c)가 있긴 한데 아직 많지 않고, 성능이 안뽑히는 것 같음.
- 해볼만한 주제인 것 같은데 일단 기본 툴부터 빠르게 익혀보자
