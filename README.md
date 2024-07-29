# ⌨️ 타이핑 테스트 (Typing Test) 프로젝트
## 프로젝트 개요
타이핑 테스트 프로젝트는 사용자의 타자 속도와 정확도를 측정하는 프로그램을 제작하는 프로젝트입니다.  

이 프로젝트는 Python 프로그래밍, 문자열 처리, 알고리즘 설계 및 구현, 멀티플레이어 기능 개발 등을 사용하였으며,

주어진 문장을 입력하는 시간과 정확도를 분석하여 단어 당 분당 타수(WPM)와 정확도(Accuracy)를 계산합니다. 

## 사용된 언어
- Python

## 주요 기능
- **문단 선택 및 필터링**:
  - `pick(paragraphs, select, k)`: 조건에 맞는 k번째 문단을 선택
  - `about(subject)`: 주어진 주제 단어들이 포함된 문단을 필터링하는 함수

- **정확도 및 타자 속도 계산**:
  - `accuracy(typed, source)`: 사용자가 입력한 문장과 원본 문장을 비교하여 정확도를 계산
  - `wpm(typed, elapsed)`: 입력된 문자열을 기준으로 분당 타수(WPM)를 계산

- **자동 교정 및 최소 편집 거리 계산**:
  - `autocorrect(typed_word, word_list, diff_function, limit)`: 사용자가 입력한 단어를 주어진 단어 리스트와 비교하여 가장 유사한 단어로 자동 교정
  - `feline_fixes(typed, source, limit)`: 최소한의 문자 교체를 통해 두 단어 사이의 편집 거리를 계산
  - `minimum_mewtations(typed, source, limit)`: 주어진 제한 내에서 최소 편집 거리를 계산

- **멀티플레이어 기능**:
  - `report_progress(typed, prompt, user_id, upload)`: 사용자 ID와 진행 상황을 서버에 업로드하고 현재 진행 상황을 반환
  - `time_per_word(words, times_per_player)`: 각 단어를 타이핑하는 데 걸린 시간을 계산하여 반환
  - `fastest_words(match)`: 각 단어를 가장 빨리 타이핑한 플레이어를 반환

## 결과 / 결론
- 타자 속도 및 정확도 분석을 통한 성과 측정
- Python을 활용한 입력 데이터 처리 및 분석
- 사용자의 타자 능력 향상을 위한 피드백 제공
- 멀티플레이어 타자 게임 구현 및 진행 상황 추적
