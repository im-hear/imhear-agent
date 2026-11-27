# imhear-agent

ImHear의 Python · FastAPI · GMS · pgvector 저장소입니다. 담당 범위는 A의 Market Agent·RAG·색인, B의 Trading Agent·Order Harness, 공동 Intent Router·GMS Client입니다.

## 계약과 검증

Tool은 Pydantic 입력·출력 검증을 거친다. 현재 가격은 Spring 금융 Tool에서 받고, Trading Agent는 주문 초안만 요청한다.

[Agent 평가 기준](docs/evaluation.md)에 따라 Tool 계약, 응답 근거와 권한 경계를 검증한다.

현재 폴더에는 협업 설정이 들어 있습니다. 서비스 코드와 테스트 하네스가 추가되면 이 위치에 설치, 실행, 검사 명령을 기록합니다. 네 저장소를 함께 여는 경우 상위 작업공간의 `docs/architecture/README.md`와 `docs/team-workflow.md`에서 공용 설계와 PR 흐름을 확인할 수 있습니다.

[에이전트 개발 지침](AGENTS.md)
