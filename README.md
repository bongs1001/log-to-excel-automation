# log-to-excel-automation
Automates the conversion of text-based meeting or mentoring logs into structured Excel files.

# Log-to-Excel Automation

텍스트 형식의 멘토링/회의 일지를 자동으로 정리하여 Excel 파일로 변환하는 프로젝트입니다.  
(PoC 수준의 개인 프로젝트로 시작했으며, 반복 업무를 줄이기 위한 자동화 도구입니다.)

## ✨ Features

텍스트 로그(txt)를 읽어 자동으로 구조화

Gemini API를 활용하여 요약 → Excel 변환

날짜/참석자/주요 내용/결정/액션아이템 정리

다수의 파일을 한 번에 처리 가능

## 📂 Project Structure

data/ : 샘플 txt 파일

outputs/ : 변환된 Excel 결과 (기본: log_to_excel_output.xlsx)

src/ : 코드 (메인 스크립트 main.py)

## 🚀 Getting Started
### 1. Clone & Install
git clone https://github.com/bongs1001/log-to-excel-automation.git
cd log-to-excel-automation
pip install -r requirements.txt

### 2. 환경변수 설정 (.env)

루트 폴더에 .env 파일을 생성하고 아래 내용을 추가하세요:

GEMINI_API_KEY=your_gemini_api_key_here


GEMINI_API_KEY는 Google AI Studio
에서 발급받을 수 있습니다.

### 3. Run
python src/main.py


입력: data/*.txt

출력: outputs/log_to_excel_output.xlsx

## 🛠 Tech Stack

Python 3.10+

Pandas, OpenPyXL

Google Generative AI (Gemini API)

dotenv

## 📊 Example

입력:

2025.08.25 팀 회의
참석자: 김A, 이B, 박C
내용: 프로젝트 일정 논의


출력 (Excel):
| 일자 및 시간    | 참석자        | 내용         | 결정사항         |
| ---------- | ---------- | ---------- | ------------ |
| 2025-08-25 | 김A, 이B, 박C | 프로젝트 일정 논의 | 로그 파서 PoC 진행 |
