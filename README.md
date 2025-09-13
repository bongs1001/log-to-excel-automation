# log-to-excel-automation
Automates the conversion of text-based meeting or mentoring logs into structured Excel files.

# Log-to-Excel Automation

텍스트 형식의 멘토링/회의 일지를 자동으로 정리하여 Excel 파일로 변환하는 프로젝트입니다.  
(PoC 수준의 개인 프로젝트로 시작했으며, 반복 업무를 줄이기 위한 자동화 도구입니다.)

## ✨ Features
- txt 파일을 읽어와 자동으로 구조화
- Excel로 변환하여 날짜/참여자/내용을 정리
- 다수의 파일을 한 번에 처리 가능

## 📂 Project Structure
- `data/` : 샘플 txt 파일
- `outputs/` : 변환된 Excel 예시
- `src/` : 코드

## 🚀 Getting Started
```bash
git clone https://github.com/username/log-to-excel-automation.git
cd log-to-excel-automation
pip install -r requirements.txt
python src/main.py
