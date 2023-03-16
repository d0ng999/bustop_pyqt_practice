# PyQT를 활용한 버스 탑승 APP
2023.03.15 제작

## 개발목적
- 특정 버스의 탑승 대기인원을 사전에 알려 버스 정류장에서의 멈춤 유무를 사전에 전달하기 위함

## 기술스택
- Python 3.11.2
- PyQt5
    - pymysql 모듈 사용
- Qt Designer
- MySQL

1. Qt Designer을 활용한 ui 제작
![QtDesigner](https://raw.githubusercontent.com/PKNU-IOT3/bustop_pyqt_practice/main/images/QtDesigner.png)
2. MySQL DB 작성
![MySQL](https://raw.githubusercontent.com/PKNU-IOT3/bustop_pyqt_practice/main/images/mysql.png)
3. Python으로 기능 작성
![실행화면1](https://raw.githubusercontent.com/PKNU-IOT3/bustop_pyqt_practice/main/images/%EC%8B%A4%ED%96%89%ED%99%94%EB%A9%B4_1.png)
![실행화면2](https://raw.githubusercontent.com/PKNU-IOT3/bustop_pyqt_practice/main/images/%EC%8B%A4%ED%96%89%ED%99%94%EB%A9%B4_2.png)

### 로직
- 버스의 탑승대기/탑승취소 버튼을 통해 해당 버스 탑승 인원 카운팅
- 카운팅된 인원을 DB로 저장
- DB에서 변경되는 탑승인원(bus_cnt)의 내용도 앱으로 실시간 반영

## 23.03.16 프로젝트 수정
- RadioButton을 사용하여 탑승 대기 / 탑승 취소 버튼을 각각 3개에서 1개로 축소
- UI 수정
![QtDesigner](https://raw.githubusercontent.com/PKNU-IOT3/bustop_pyqt_practice/main/images/QtDesigner_modify.png)
![실행화면](https://raw.githubusercontent.com/PKNU-IOT3/bustop_pyqt_practice/main/images/%EC%8B%A4%ED%96%89%ED%99%94%EB%A9%B4_modify.png)