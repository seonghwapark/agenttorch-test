# 🐺 agenttorch-test

AgentTorch 프레임워크를 활용한 포식자-피식자(Predator-Prey) 생태계 시뮬레이션.

## 개요

격자 환경에서 포식자·피식자·풀의 상호작용을 에이전트 기반 모델로 시뮬레이션한다.
AgentTorch의 기본 기능을 탐색하고 학습하기 위한 테스트 프로젝트.

## 시뮬레이션 구성

| 요소 | 수량 |
|------|------|
| 포식자 (Predator) | 40 |
| 피식자 (Prey) | 80 |
| 풀 패치 (Grass) | 450 |
| 격자 크기 | 18 × 25 |

## 주요 기능

- 포식자의 사냥(Hunt), 이동(Move) 행동 모델링
- 피식자의 먹이(Eat), 이동(Move) 행동 모델링
- 풀의 성장(Grow) 사이클
- 시뮬레이션 결과 GIF/MP4 시각화

## 기술 스택

- Python 3.11
- AgentTorch v0.4
- PyTorch, NumPy
- YAML 기반 설정 관리

## 실행 방법

```bash
python main.py
```

결과는 `plots/` 폴더에 저장된다.

## 프로젝트 구조

```
agenttorch-test/
├── main.py             # 시뮬레이션 실행
├── config.yaml         # 파라미터 설정
├── substeps/           # 행동 모듈 (hunt, move, eat, grow)
├── helpers/            # 유틸리티
├── data/               # 초기 상태 데이터
├── media/              # 시뮬레이션 결과 영상
└── docs/               # 문서 및 튜토리얼
```

## 결과 미리보기

![Predator-Prey Simulation](media/predator-prey.gif)
