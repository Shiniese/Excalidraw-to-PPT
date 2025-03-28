# **Excalidraw-to-PPT**

![Python](https://img.shields.io/badge/python-3.12-blue) ![License](https://img.shields.io/badge/license-MIT-green)

`.excalidraw` 파일을 파워포인트 프레젠테이션(PPT)으로 변환하는 과정을 자동화하는 파이썬 도구입니다. `.excalidraw` 파일에 포함된 이미지를 추출하여 이를 PNG 파일로 저장하고, 깔끔하게 정리된 형식으로 파워포인트 슬라이드에 배치합니다.

---

## **기능**
- `.excalidraw` 파일에서 base64 인코딩된 이미지 자동 추출.
- 추출한 이미지를 전용 폴더에 개별 PNG 파일로 저장.
- 모든 이미지를 그리드 레이아웃으로 배치한 파워포인트 프레젠테이션 생성.
- 단일 디렉토리에서 다수의 `.excalidraw` 파일 지원.

---

## **설치**

1. **리포지토리 복제**
   ```bash
   git clone https://github.com/Shiniese/Excalidraw-to-PPT.git
   cd Excalidraw-to-PPT
   ```

2. **종속성 설치**
   `pip`를 사용하여 필요한 파이썬 라이브러리를 설치:
   ```bash
   pip install python-pptx Pillow
   ```

3. **당신의 Excalidraw 파일 배치**
   `.excalidraw` 파일을 프로젝트 디렉토리에 복사.

---

## **사용 방법**

1. 스크립트 실행:
   ```bash
   python excalidraw_to_ppt.py
   ```

2. 도구는 아래와 같은 작업을 수행:
   - 현재 디렉토리 안에 있는 모든 `.excalidraw` 파일에서 이미지를 추출.
   - 각 파일 이름과 동일한 하위 폴더에 이미지를 저장.
   - 해당 이미지들을 정렬하여 포함한 파워포인트 파일 (`excalidraw_to_ppt.pptx`)을 생성.

---

## **예시**

#### 입력:
당신이 세 가지 `.excalidraw` 파일을 가지고 있다고 가정:
- `diagram1.excalidraw`
- `diagram2.excalidraw`
- `notes.excalidraw`

#### 출력:
- `diagram1/` 폴더에는 추출된 이미지 (예: `diagram1-1.png`, `diagram1-2.png`).
- `diagram2/` 폴더에는 추출된 이미지 (예: `diagram2-1.png`, `diagram2-2.png`).
- `notes/` 폴더에는 추출된 이미지 (예: `notes-1.png`).

각 `.excalidraw` 파일에 대한 이미지가 잘 정리된 슬라이드를 포함한 파워포인트 파일(`excalidraw_to_ppt.pptx`)이 생성됩니다.

---

## **필요한 의존성**

다음 파이썬 라이브러리들이 필요:
- `python-pptx` (파워포인트 프레젠테이션 제작용)
- `Pillow` (이미지 처리용)
- `os` 및 `json` (내장 파이썬 모듈)

다음 명령어로 설치 가능:
```bash
pip install python-pptx Pillow
```

---

## **협력 방법**

이 프로젝트에 기여하고 싶다면:
1. 리포지토리를 포크.
2. 새로운 브랜치 생성 (`git checkout -b feature/YourFeatureName`).
3. 변경 사항 커밋 (`git commit -m "Add some feature"`).
4. 브랜치에 푸시 (`git push origin feature/YourFeatureName`).
5. 풀 리퀘스트 열기.

---

## **라이선스**

이 프로젝트는 **MIT License**에 따라 라이선스를 받았습니다. 자세한 내용은 [LICENSE](https://github.com/Shiniese/Excalidraw-to-PPT/blob/main/LICENSE) 파일을 참조하십시오.

---

## **크레딧**

- 디자인 도구와 프레젠테이션 간의 워크플로 자동화 필요에 의해 영감을 얻음.
- `python-pptx` 및 `Pillow`와 같은 파이썬 라이브러리에 의해 구동됨.
