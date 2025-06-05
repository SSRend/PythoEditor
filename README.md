# 🖼️ PythoEditor

**PythoEditor**는 간단한 GUI 기반의 이미지 편집 도구입니다.  
초보자도 직관적으로 사용할 수 있도록 설계되었으며, 주요 이미지 필터와 효과를 손쉽게 적용할 수 있습니다.

![PythoEditor 메인 화면](main_menu.png)  
![편집 화면 예시](edit_mode.png)

## 🎬 소개 영상
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/cFqQS-OgYSI/0.jpg)](https://www.youtube.com/watch?v=cFqQS-OgYSI)

클릭 시, 유튜브로 이동합니다.

---

## 🛠️ 주요 기능

- ✅ **흑백 변환**: 컬러 이미지를 간단히 흑백으로 전환  
- ✅ **밝기 조절**: 슬라이더를 통해 -255 ~ +255 범위 내에서 밝기 조절  
- ✅ **크기 조절**: 원하는 가로/세로 픽셀 입력으로 이미지 사이즈 조정  
- ✅ **회전**: 각도(정수) 입력으로 자유롭게 회전  
- ✅ **대칭 반전**: 좌우 및 상하 반전 가능  
- ✅ **색상 반전**: 이미지 색상을 반전  
- ✅ **엣지 검출**: Canny 엣지 검출로 윤곽 강조  
- ✅ **블러**: 약하게/중간/강하게 3단계 Gaussian 블러 적용  
- ✅ **채널 분리**: R, G, B 채널 각각 분리 출력  

---

## 📁 기타 기능

- 🖼️ **새 이미지 생성**: 원하는 해상도와 배경색으로 초기 이미지 생성  
- 🗑️ **이미지 삭제**: 저장된 이미지 선택 후 삭제 가능  
- 🔁 **Undo / Redo**: 편집 기록을 기반으로 되돌리기, 다시 실행 가능  
- 💾 **저장**: 현재 작업 이미지를 기존 경로에 저장  
- 🔊 **배경 음악**: 메인 화면 및 편집 화면에서 자동 재생 (main_theme.wav)  
- 🖱️ **Pygame GUI 기반**: 직관적인 마우스 인터페이스 지원

---

## 💻 실행 환경

- Python 3.10 이상 권장
- 필수 패키지:
  ```bash
  pip install pygame opencv-python numpy
  ```

> ⚠️ 실행 파일 제작 시 PyInstaller를 사용하며, `assets`, `images`, `lib` 폴더를 함께 배포해야 합니다.

---

## 📦 폴더 구조

```
PythoEditor/
├── assets/            # 배경 이미지, 사운드, 폰트 등
│   ├── title_screen.png
│   ├── edit_mode.png
│   ├── main_theme.wav
│   └── SCDream7.otf
├── images/            # 유저가 만든 이미지 저장 경로 (최대 20개)
├── lib/
│   └── edit_mode.py   # 편집 모드 메인 기능
├── main.py            # 실행 진입점
└── README.md
```

---

## 📝 사용 방법

1. `main.py`를 실행하여 메인 메뉴 진입
2. 새 이미지 생성 또는 이미지 선택 후 편집 시작
3. 좌측 기능 버튼 클릭 → 필요시 우측 입력 영역 사용
4. 편집 완료 후 [저장] 버튼 클릭

---

## 📌 미리보기

| 기능 | 이미지 예시 |
|------|--------------|
| 흑백 변환 | ![gray](docs/images/gray_sample.png) |
| 밝기 조절 | ![bright](docs/images/bright_sample.png) |
| 엣지 검출 | ![edge](docs/images/edge_sample.png) |

> 위 이미지는 `docs/images`에 저장해 함께 배포하면 됩니다.

---

## 📣 라이선스

본 프로젝트는 MIT 라이선스를 따릅니다. 자유롭게 사용하고, 수정 및 배포할 수 있습니다.

---

**즐거운 이미지 편집 되세요!** 🎨
