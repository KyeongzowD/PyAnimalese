# PyAnimalese에 대하여
동물의 숲 NPC 목소리로 문장을 읽어주는 프로그램을 함수로 변경한 코드입니다.

## 지원 언어
- 한국어

## 원리
1. 한글로 문자열을 입력 받는다.
2. 문자열을 순회하면서 자모를 분리해서 초성만 얻어낸다.
3. 미리 녹음해둔 해당 초성의 발음파일(e.g. 'ㄱ'은 '그' 처럼 어중간하게 발음함)을 가져온다.
4. 피치를 높인다. 이 때, 랜덤으로 피치 값을 조절한다.
5. 하나로 합쳐서 재생(저장)한다.

## 실행하기
- 방법1: pyanimalese_cli.py를 직접 실행합니다. 이때, sources 폴더가 필요하며 아래의 디펜던시 패키지를 설치해야합니다.
- 방법2: 릴리즈 버전을 다운로드하여 GUI로 사용합니다. [바로가기](https://github.com/hwi-middle/PyAnimalese/releases)

<b>주의: 두 방법 모두 ffmpeg이 설치되어있어야합니다.</b>

## 디펜던시
- [Pydub](https://github.com/jiaaro/pydub)
- [Jamo](https://github.com/JDongian/python-jamo)
- [PyAudio](https://people.csail.mit.edu/hubert/pyaudio/)

## 디펜던시 패키지 설치 (Windows 기준)
```pip install -r requirements.txt```

```pipwin install pyaudio```

<b>주의: PyAudio는 pipwin으로 별도로 설치해야합니다.</b>

