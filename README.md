# 2026-1-BDA
2026년 1학기 '빅데이터분석프로그래밍' 교과목

## 온라인 출석과 수업 참여
- [A반(QA) 수요일 오전](https://docs.google.com/spreadsheets/d/1D6ayWWOMeVnYbkdMYzPTb6pRjdNcvLFk4VPmn_ylpus/edit?usp=sharing)
- [B반(QB) 수요일 오후](https://docs.google.com/spreadsheets/d/1eSEnDMEoiSUiUgyeKz_xyt1tmn8EPJ3cRPKXZdKE7i4/edit?usp=sharing)

## 시험 일정
- 중간고사 2026/4/22수 오후 1:00 ~ 2:00
- 기말고사 2026/6/17수 오후 1:00 ~ 2:00

## 타이타닉 열(변수) 설명
- survived : 0 = 사망, 1 = 생존
- pclass : 1 = 1등석, 2 = 2등석, 3 = 3등석
- sex : male = 남성, female = 여성
- age : 나이
- sibsp : 타이타닉 호에 동승한 자매 / 배우자의 수
- parch : 타이타닉 호에 동승한 부모 / 자식의 수
- fare : 티켓 요금
- embarked : 탑승지, C = 셰르부르, Q = 퀸즈타운, S = 사우샘프턴
- class : First = 1등석, Second = 2등석, Third = 3등석
- who : 남/여/아이, 'man', 'woman', 'child'
- adult_male : 남자 어른, True/False
- deck : 방 위치, 'A', 'B', 'C', 'D', 'E', 'F', 'G', NaN
- embark_town : 탑승지
- alive : 생존, yes/no
- alone : 1인 탑승, True/False

### deck(방 위치)
- ![image](https://github.com/user-attachments/assets/8be11782-751f-4934-ac37-57930fbbc1f3)

## 데이터분석 프로그래밍(4-5명 팀 과제)
- 다음 두 과제를 모두 수행
  - 과제1: 지정 데이터(titanic1309.csv) 분석: 타이타닉호 데이터 분석
  - 과제2: 자유 데이터 분석: 공공 데이터 분석 선택
- A반 5/27(수), B반 5/27(수) 수업에서 발표
  - 주피터노트북(발표 내용과 코드)으로 발표(발표시간은 약 10~15분)
- 데이터 공모전에 참가하는 방향으로 자유 데이터 활용
  - [교통데이터 공모전](https://www.bigdata-transportation.kr/pageant/dashboard/CMPE_000000000020041)

## 지도 시각화 수업 참조
- [웹참조](https://pjh09050.tistory.com/11)
  
## 가로로 데이터프레임 출력 함수
```Python
from IPython.display import display_html
def display_side_by_side(*args):
    """여러 데이터프레임 비교가 쉽게 옆쪽으로 표시한다"""
    html_str=''
    for df in args:
        html_str += df.to_html() + '&nbsp;'*4
    display_html(html_str.replace('table','table style="display:inline"'), raw=True)
```
## Google Colab 셀 복사 및 붙여넣기 단축키

- 🔹 셀 복사 & 붙여넣기 단축키

| 작업 | Windows / Linux | Mac |
|------|----------------|-----|
| **셀 복사** | `Ctrl + M, C` | `Cmd + M, C` |
| **셀 붙여넣기** | `Ctrl + M, V` | `Cmd + M, V` |

- 🔹 추가로 유용한 셀 관련 단축키

| 작업 | Windows / Linux | Mac |
|------|----------------|-----|
| **셀 잘라내기** | `Ctrl + M, X` | `Cmd + M, X` |
| **셀 삭제** | `Ctrl + M, D` | `Cmd + M, D` |
| **새 코드 셀 추가** | `Ctrl + M, B` | `Cmd + M, B` |
| **셀 실행** | `Shift + Enter` | `Shift + Enter` |
| **셀 실행 후 아래에 새 셀 추가** | `Alt + Enter` | `Alt + Enter` |

> 💡 `Ctrl + M` (`Cmd + M` on Mac)을 누른 후 해당 키를 입력하면 실행됩니다.  
> Colab에서 셀을 빠르게 조작할 때 활용해 보세요! 🚀

