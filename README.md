# 생명과학 시뮬레이션 (BiologyClass)

고등학교 생명과학 수업에서 쓰는 인터랙티브 시뮬레이션 모음입니다.
학생이 직접 누르고 바꿔 보며 세포, 물질대사, 유전, 진화를 탐구할 수 있습니다.

- 별도 설치나 서버 없이 **HTML 파일만으로 동작**합니다.
- PC와 태블릿 화면에 맞춰 제작되었습니다.
- 수업에서는 자료별 QR 코드로 각 페이지에 접속해 사용합니다.

## 시뮬레이션 목록

시작 페이지는 [`index.html`](index.html)입니다.

### 세포와 구성 물질
| 파일 | 내용 | 확인 문제 |
|---|---|:---:|
| [`Microscope.html`](Microscope.html) | 현미경 사용법, 접안·대물마이크로미터로 세포 크기 측정 | ✅ |
| [`CellStructure.html`](CellStructure.html) | 원핵세포·진핵세포 비교, 세포소기관의 구조와 기능 | ✅ |
| [`Biomolecules.html`](Biomolecules.html) | 탄수화물·지질·단백질·핵산, 3D 구조, 가상 영양소 검출 실험 | ✅ |

### 효소와 물질대사
| 파일 | 내용 | 확인 문제 |
|---|---|:---:|
| [`EnzymeInhibitor.html`](EnzymeInhibitor.html) | 억제제 종류에 따른 기질 농도–반응 속도 그래프 비교 | |
| [`Photosynthesis.html`](Photosynthesis.html) | 세포호흡(해당 과정~산화적 인산화), 발효, 명반응, 캘빈 회로 | ✅ |

### 유전 정보와 세포 분열
| 파일 | 내용 | 확인 문제 |
|---|---|:---:|
| [`CentralDogma.html`](CentralDogma.html) | DNA 구조·복제부터 전사, RNA 가공, 번역, 돌연변이, 발현 조절까지 2D·3D 통합 시뮬레이션 | ✅ |
| [`DNARep.html`](DNARep.html) | 반보존적 복제, 선도가닥·지연가닥 합성 | |
| [`RNATrans.html`](RNATrans.html) | mRNA 서열 입력 → 코돈·tRNA·라이보솜으로 폴리펩타이드 합성 | |
| [`CellDivision.html`](CellDivision.html) | 체세포 분열과 감수 분열 비교, 염색체 변화 관찰 | |

### 진화와 분류
| 파일 | 내용 | 확인 문제 |
|---|---|:---:|
| [`RevSim.html`](RevSim.html) | 세대에 따른 대립유전자 빈도 변화 | |
| [`Dis.html`](Dis.html) | 가상 생물 7종을 비교해 계통수 세우기, 새 생물 분류 | |

### 기타
| 파일 | 내용 |
|---|---|
| [`metabolism_simulation_scaffold.html`](metabolism_simulation_scaffold.html) | 세포와 물질대사 시뮬레이션 (현재 `index.html`에는 연결되어 있지 않음) |

## 사용 방법

1. 브라우저로 `index.html`을 열거나, 원하는 시뮬레이션 HTML 파일을 바로 엽니다.
2. 수업에서는 각 파일 주소를 QR 코드로 만들어 학생 태블릿으로 접속합니다.

로컬에서 확인할 때는 파일을 더블클릭해서 열어도 되고, 간단한 정적 서버를 띄워도 됩니다.

```bash
# 예: Python이 설치되어 있다면
python -m http.server 8000
# 브라우저에서 http://localhost:8000 접속
```

## 앞으로의 계획: 퀴즈 결과 수집 (개발 중)

수업 시간에 학생들의 확인 문제 결과를 모아 선생님 화면에서 볼 수 있도록 백엔드를 붙이는 작업을 준비하고 있습니다.

- **학생 개인정보(실명·학번 등)는 받지 않는 구조**를 원칙으로 합니다.
- 기존 시뮬레이션은 서버 없이도 지금처럼 그대로 동작하도록 유지합니다.
- 실제 수업 도입 전에 학교의 확인을 거칠 예정입니다.

설계 내용은 [`BACKEND_PLAN.md`](BACKEND_PLAN.md)에 정리되어 있습니다.

## 제작

ⓒ 이재빈, 광덕고등학교 · 도움: 용용
