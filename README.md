# 에이전트형 코딩 보조 도구를 활용한 명세 기반 개발(Spec-Driven Development)

이 저장소는 DeepLearning.AI의 ​​'명세 기반 개발(Spec-Driven Development)' 강의를 위한 실습용 코드를 포함하고 있습니다. 각 비디오 폴더에는 해당 강의를 따라 실습하는 데 필요한 프로젝트의 전체 상태가 담겨 있습니다.

## 기타 DeepLearning.AI 리소스
> :mortar_board: **학습 계속하기** → [DeepLearning.AI의 ​​모든 강의 살펴보기](https://www.deeplearning.ai/courses/) — AI의 미래를 만들어가는 전문가들이 직접 가르치는 강의입니다. 다음 학습 과정을 찾아보세요.
>
> :computer: **더 많은 강의 자료 살펴보기** → [DeepLearning.AI 강의 자료 저장소](https://github.com/https-deeplearning-ai/deeplearning-ai)를 방문하여 다양한 강의의 노트북, 프로젝트, 학습 노트 등을 확인해 보세요.

## 저장소 사용 방법

이 강의를 수강하는 가장 간단한 방법은 'Video 5'부터 시작하여 각 비디오의 내용을 따라가며 프로젝트를 직접 구축해 보는 것입니다.

각 `VideoNN_*` 폴더에는 해당 비디오가 **시작되는 시점**의 AgentClinic 프로젝트 상태(스냅샷)가 포함되어 있습니다. 이전 비디오를 완료하지 않고도 특정 비디오부터 바로 시작할 수 있도록 각 단계별 폴더가 제공되므로, 매번 폴더를 복사할 필요는 없습니다. 특정 비디오 단계부터 새로 시작하고 싶다면, 해당 폴더를 본인의 작업 디렉토리로 복사하기만 하면 됩니다:

```bash
cp -r Video06_Feature_Specification/ my-agentclinic/
cd my-agentclinic
npm install
```

## 비디오 개요

각 비디오 폴더에는 해당 비디오를 위한 **완전한 시작 코드(starter code)**와 강의 중 사용된 **모든 프롬프트**가 포함되어 있습니다.

| 폴더 | 비디오 | 시작 시점의 상태 |
|--------|-------|--------------------------|
| Video05_Creating_the_Constitution | Creating the Constitution (헌장(Constitution) 생성) | 빈 프로젝트 스캐폴드 (package.json, tsconfig.json, src/index.ts) |
| Video06_Feature_Specification | Feature Specification (기능 사양 정의) | 헌장(Constitution)이 포함된 상태 (specs/mission.md, tech-stack.md, roadmap.md) |
| Video07_Feature_Implementation | 기능 구현 | 기본 원칙(Constitution) + Phase 1 기능 명세(plan.md, requirements.md, validation.md) |
| Video08_Feature_Validation | 기능 검증 | 레이아웃 컴포넌트를 포함한 Phase 1 "Hello Hono" 완전 구현 |
| Video09_Project_Replanning | 프로젝트 재계획 | Phase 1을 main 브랜치에 병합, 재계획 준비 완료 |
| Video10_The_second_feature_phase | 두 번째 기능 단계 | 재계획 완료 (테스트, 반응형 디자인, 변경 로그(changelog) 스킬 추가) |
| Video11_The_MVP | MVP | Phase 2 "Agents & Ailments" 병합, MVP 스프린트를 위한 전체 앱 준비 완료 |
| Video12_Legacy_support | 레거시 지원 | MVP 완전 구현, 레거시 SDD 도입 준비 완료 |
| Video13_Build_your_own_workflow | 나만의 워크플로 구축 | 레거시 기본 원칙(constitution) 재구축 + 피드백 폼 기능 구현 |
| Video14_Agents_replaceability | 에이전트 교체 가능성 | 피드백 폼 병합, 기능 명세 스킬 생성, 다음 기능 명세 초안 작성, 리서치 노트를 포함한 백로그(backlog) 구성 |

Video 2~4(명세 주도 개발의 이유, 워크플로 개요, 설정)는 개념적인 내용으로, 별도의 스타터 코드가 제공되지 않습니다.

## 기타 디렉토리

- **`prompts/`** -- 모든 비디오 프롬프트를 한곳에 모아둔 폴더입니다. 각 파일에는 해당 비디오의 번호가 매겨진 프롬프트가 포함되어 있습니다. 각 `VideoNN_*/` 폴더 안에도 `prompts.md`라는 이름으로 사본이 들어 있습니다.
- **`skills/`** -- 과정 중에 개발된 재사용 가능한 에이전트 스킬(changelog, feature-spec)입니다.
- **`example_specs/`** -- 과정에서 참조된 예시 명세 문서입니다.

## 사전 요구 사항

- Node.js (v18 이상)
- Git
- 코딩 에이전트 (이 과정에서는 Claude Code를 사용하지만, 워크플로는 특정 에이전트에 종속되지 않음)
- IDE 또는 에디터 (이 과정에서는 [WebStorm](https://www.jetbrains.com/webstorm/download/)을 사용함)
