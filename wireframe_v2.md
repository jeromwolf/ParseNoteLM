# ParseNoteLM UI 와이어프레임 v2
## (NotebookLM 스타일 참고)

## 🏠 메인 대시보드 (프로젝트 목록)

```
┌─────────────────────────────────────────────────────────────┐
│ 🔍 ParseNoteLM                              김철수 👤 [⚙️]   │
└─────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────┐
│                                                             │
│               ParseNoteLM에 오신 것을 환영합니다             │
│                                                             │
│                    [+ 새 프로젝트 만들기]                   │
│                                                             │
│  ┌─────────────────┐ ┌─────────────────┐ ┌─────────────────┐ │
│  │ 📚              │ │ 📊              │ │ 📄              │ │
│  │                 │ │                 │ │                 │ │
│  │ AI 연구논문 모음 │ │ 데이터분석 자료 │ │ 회사업무 문서   │ │
│  │                 │ │                 │ │                 │ │
│  │ 2025. 5. 20.    │ │ 2025. 5. 15.    │ │ 2025. 5. 10.    │ │
│  │ • 3개 문서      │ │ • 2개 문서      │ │ • 1개 문서      │ │
│  │                 │ │                 │ │                 │ │
│  └─────────────────┘ └─────────────────┘ └─────────────────┘ │
│                                                             │
│  ┌─────────────────┐ ┌─────────────────┐ ┌─────────────────┐ │
│  │                 │ │                 │ │      + 새       │ │
│  │                 │ │                 │ │   프로젝트      │ │
│  │   (비어있음)     │ │   (비어있음)     │ │                 │ │
│  │                 │ │                 │ │   최대 3개까지   │ │
│  │                 │ │                 │ │                 │ │
│  │                 │ │                 │ │                 │ │
│  │                 │ │                 │ │                 │ │
│  └─────────────────┘ └─────────────────┘ └─────────────────┘ │
│                                                             │
│                        사용량: 프로젝트 3/3개                │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

## 📂 프로젝트 내부 (3단 레이아웃)

```
┌─────────────────────────────────────────────────────────────┐
│ ← ParseNoteLM > AI 연구논문 모음           김철수 👤 [⚙️]    │
└─────────────────────────────────────────────────────────────┘

┌──────────────┬─────────────────────────┬─────────────────────┐
│ 📁 소스      │   📖 메인 뷰어          │ 🤖 노트북 가이드     │
│              │                         │                     │
│ ✅ 모든 소스  │ ┌─────────────────────┐ │ ┌─────────────────┐ │
│   • 3개 소스 │ │                     │ │ │ 📄 문서 정보     │ │
│              │ │ Research Paper 1    │ │ │                 │ │
│ 📄 research_ │ │                     │ │ │ 파일명:         │ │
│    paper1.pdf│ │ Abstract:           │ │ │ research_paper1 │ │
│ ✅ 선택됨    │ │                     │ │ │ .pdf            │ │
│              │ │ This paper presents │ │ │                 │ │
│ 📄 machine_  │ │ a novel approach to │ │ │ 크기: 2.3MB     │ │
│    learning.pdf│ │ improve deep       │ │ │ 페이지: 15      │ │
│ 2025.5.18    │ │ learning accuracy... │ │ │ 업로드: 5/20    │ │
│              │ │                     │ │ │                 │ │
│ 📄 deep_     │ │ 1. Introduction     │ │ └─────────────────┘ │
│    learning.txt│ │                     │ │                     │
│ 2025.5.15    │ │ Recent advances in  │ │ ┌─────────────────┐ │
│              │ │ artificial intelli- │ │ │ 💬 이 문서에     │ │
│ [+ 소스 추가]│ │ gence have shown... │ │ │    질문하기      │ │
│              │ │                     │ │ │                 │ │
│              │ │ 2. Methodology      │ │ │ 예: 이 논문의    │ │
│              │ │                     │ │ │ 핵심 기술은?     │ │
│              │ │ We propose a new    │ │ │                 │ │
│              │ │ architecture...     │ │ │ [질문하기]      │ │
│              │ │                     │ │ └─────────────────┘ │
│              │ └─────────────────────┘ │                     │
│              │                         │ ┌─────────────────┐ │
│              │ [🔍 문서 내 검색]        │ │ 📌 하이라이트    │ │
│              │                         │ │                 │ │
│              │                         │ │ • Introduction  │ │
│              │                         │ │ • Methodology   │ │
│              │                         │ │ • Results       │ │
│              │                         │ │                 │ │
│              │                         │ └─────────────────┘ │
│              │                         │                     │
└──────────────┴─────────────────────────┴─────────────────────┘
```

## 💬 채팅 모드 (질의응답)

```
┌─────────────────────────────────────────────────────────────┐
│ ← ParseNoteLM > AI 연구논문 모음 > 채팅     김철수 👤 [⚙️]  │
└─────────────────────────────────────────────────────────────┘

┌──────────────┬─────────────────────────┬─────────────────────┐
│ 📁 소스      │   💬 채팅                │ 🤖 노트북 가이드     │
│              │                         │                     │
│ ✅ 모든 소스  │ ┌─────────────────────┐ │ ┌─────────────────┐ │
│   • 3개 소스 │ │                     │ │ │ 💡 AI 어시스턴트 │ │
│              │ │                     │ │ │                 │ │
│ 📄 research_ │ │ 👤 사용자                    방금           │ │
│    paper1.pdf│ │                                             │ │
│ 2025.5.20    │ │ 이 논문들의 주요 결론을 요약해주세요         │ │
│              │ └─────────────────────┘ │ │                 │ │
│ 📄 machine_  │ ┌─────────────────────┐ │ │ 💬 시작해보세요: │ │
│    learning.pdf│ │                     │ │ │                 │ │
│ 2025.5.18    │ │ 🤖 AI 어시스턴트            2분 전         │ │
│              │ │                                             │ │
│ 📄 deep_     │ │ 업로드하신 AI 연구논문들의 주요 결론은      │ │
│    learning.txt│ │                                             │ │
│ 2025.5.15    │ │ 다음과 같습니다:                            │ │
│              │ │                                             │ │
│ [+ 소스 추가]│ │ 1. **딥러닝 성능 향상** (research_paper1)   │ │
│              │ │    - 새로운 아키텍처로 정확도 15% 개선      │ │
│              │ │                                             │ │
│              │ │ 2. **머신러닝 효율성** (machine_learning)   │ │
│              │ │    - 계산 비용 30% 절감하는 알고리즘        │ │
│              │ │                                             │ │
│              │ │ 3. **실무 적용** (deep_learning.txt)        │ │
│              │ │    - 산업계 도입 사례 및 성과 분석          │ │
│              │ │                                             │ │
│              │ │ 📚 출처: research_paper1.pdf, machine_     │ │
│              │ │ learning.pdf, deep_learning.txt             │ │
│              │ └─────────────────────┘ │                     │
│              │                         │                     │
│              │ ┌─────────────────────┐ │                     │
│              │ │ 문서에 대해 질문     │ │                     │
│              │ │ 하세요...          [📤]     │                     │
│              │ └─────────────────────┘ │                     │
│              │                         │                     │
│              │ 💡 제안 질문:                                   │
│              │ • 각 논문의 핵심 기술은?                        │
│              │ • 연구 방법론 비교해줘                          │
│              │ • 한계점과 개선사항은?                          │
│              │                                                 │
└──────────────┴─────────────────────────┴─────────────────────┘
```

## 📄 개별 문서 뷰

```
┌─────────────────────────────────────────────────────────────┐
│ ← ParseNoteLM > AI 연구논문 모음 > research_paper1.pdf      │
└─────────────────────────────────────────────────────────────┘

┌──────────────┬─────────────────────────┬─────────────────────┐
│ 📁 소스      │   📖 문서 뷰어           │ 🤖 노트북 가이드     │
│              │                         │                     │
│ ✅ 모든 소스  │ ┌─────────────────────┐ │ ┌─────────────────┐ │
│   • 3개 소스 │ │                     │ │ │ 📄 문서 정보     │ │
│              │ │ Research Paper 1    │ │ │                 │ │
│ 📄 research_ │ │                     │ │ │ 파일명:         │ │
│    paper1.pdf│ │ Abstract:           │ │ │ research_paper1 │ │
│ ✅ 선택됨    │ │                     │ │ │ .pdf            │ │
│              │ │ This paper presents │ │ │                 │ │
│ 📄 machine_  │ │ a novel approach to │ │ │ 크기: 2.3MB     │ │
│    learning.pdf│ │ improve deep       │ │ │ 페이지: 15      │ │
│ 2025.5.18    │ │ learning accuracy... │ │ │ 업로드: 5/20    │ │
│              │ │                     │ │ │                 │ │
│ 📄 deep_     │ │ 1. Introduction     │ │ └─────────────────┘ │
│    learning.txt│ │                     │ │                     │
│ 2025.5.15    │ │ Recent advances in  │ │ ┌─────────────────┐ │
│              │ │ artificial intelli- │ │ │ 💬 이 문서에     │ │
│ [+ 소스 추가]│ │ gence have shown... │ │ │    질문하기      │ │
│              │ │                     │ │ │                 │ │
│              │ │ 2. Methodology      │ │ │ 예: 이 논문의    │ │
│              │ │                     │ │ │ 핵심 기술은?     │ │
│              │ │ We propose a new    │ │ │                 │ │
│              │ │ architecture...     │ │ │ [질문하기]      │ │
│              │ │                     │ │ └─────────────────┘ │
│              │ └─────────────────────┘ │                     │
│              │                         │ ┌─────────────────┐ │
│              │ [🔍 문서 내 검색]        │ │ 📌 하이라이트    │ │
│              │                         │ │                 │ │
│              │                         │ │ • Introduction  │ │
│              │                         │ │ • Methodology   │ │
│              │                         │ │ • Results       │ │
│              │                         │ │                 │ │
│              │                         │ └─────────────────┘ │
│              │                         │                     │
└──────────────┴─────────────────────────┴─────────────────────┘
```

## 🔑 로그인/회원가입 (간소화)

```
┌─────────────────────────────────────────────────────────────┐
│                       ParseNoteLM                          │
│                  AI 문서 분석 서비스                        │
└─────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────┐
│                                                             │
│                  ┌─────────────────────┐                    │
│                  │                     │                    │
│                  │   🚀 시작하기        │                    │
│                  │                     │                    │
│                  │ 이메일로 계속하기    │                    │
│                  │ ┌─────────────────┐ │                    │
│                  │ │ example@email.com│ │                    │
│                  │ └─────────────────┘ │                    │
│                  │                     │                    │
│                  │ [계속하기]          │                    │
│                  │                     │                    │
│                  │ 또는               │                    │
│                  │                     │                    │
│                  │ [🔗 Google로 계속]  │                    │
│                  │                     │                    │
│                  └─────────────────────┘                    │
│                                                             │
│              무료로 시작하세요 • 프로젝트 3개 • 문서 15개    │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

## 📱 모바일 반응형

```
┌─────────────────────┐
│ ParseNoteLM   [☰]   │
├─────────────────────┤
│                     │
│ AI 연구논문 모음     │
│ ← 뒤로              │
│                     │
├─────────────────────┤
│ 📁 소스 (3)         │
│ ┌─────────────────┐ │
│ │ 📄 research_    │ │
│ │    paper1.pdf   │ │
│ │ 2.3MB • 5/20    │ │
│ └─────────────────┘ │
│ ┌─────────────────┐ │
│ │ 📄 machine_     │ │
│ │    learning.pdf │ │
│ │ 1.8MB • 5/18    │ │
│ └─────────────────┘ │
├─────────────────────┤
│ 💬 AI 어시스턴트    │
│ ┌─────────────────┐ │
│ │ 3개 문서를 분석  │ │
│ │ 했습니다. 질문해 │ │
│ │ 보세요!         │ │
│ └─────────────────┘ │
│ ┌─────────────────┐ │
│ │ 문서에 대해     │ │
│ │ 질문하세요...   │ │
│ │ [📤]           │ │
│ └─────────────────┘ │
│                     │
└─────────────────────┘
```

## 🎨 디자인 특징

### NotebookLM 스타일 채택
- **카드 기반 레이아웃**: 프로젝트를 카드로 표시
- **3단 구조**: 소스 목록 + 메인 뷰 + AI 어시스턴트
- **깔끔한 타이포그래피**: 구글 스타일의 깔끔한 디자인
- **상단 네비게이션**: 브레드크럼으로 현재 위치 표시

### 색상 및 스타일
- **화이트 베이스**: 깔끔한 흰색 배경
- **파란색 액센트**: Google Blue (#1a73e8)
- **회색 텍스트**: 부가 정보용 (#5f6368)
- **카드 섀도우**: 살짝 뜬 느낌의 그림자 효과
