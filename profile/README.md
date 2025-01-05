[Boilerplate](https://github.com/flutter-module/Boilerplate)
<br/>
<br/>
  
## 모듈별 적용 방법
```yml
# pubspec.yaml에서 아래와 같이 작성
***_module:
    git:
      url: git@github.com:flutter-module/***-module.git  # 레파지토리명
      path: ***_module  # 폴더명
      ref: v0.1.0       # 태그명
```
- 광고 : [admob_module](https://github.com/flutter-module/admob-module/blob/main/admob_module/README.md)
- 온보딩 : [onboarding](https://github.com/flutter-module/Onboarding-module/blob/main/README.md)
- 설정화면 : 
<br/>

## 최초로 적용할 때 (1회)

1. ssh 키 생성  
   터미널에서 아래 명령어 실행
   
   ```bash
   ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
   ```
   모두 엔터를 누르면 되지만 보안 강화하고 싶으면 Passphrase 암호 설정하면 됨

2. ssh 공개 키 복사
   ```bash
   cat ~/.ssh/id_rsa.pub
   ```

3. GitHub에 SSH 키 등록  
    1.	GitHub → Settings → SSH and GPG keys → New SSH key 클릭  
	2.	Title: 키를 구분할 이름 입력 (예: “M3 Key”)  
	3.	Key: id_rsa.pub의 내용(앞선 터미널 실행 결과)을 붙여넣기  
	4.	Add SSH key 클릭  

4. 연결 확인  
   터미널에서 아래 명령어를 치고, `Are you sure you want to continue connecting (yes/no/[fingerprint])?` 하면 `yes` 입력
   ```bash
   ssh -T git@github.com 
   ```

   아래와 같은 결과가 나오면 연결 성공
   ```
   Hi 유저이름! You've successfully authenticated, but GitHub does not provide shell access.
   ```
<br/>

## 모듈 만들기
1. 패키지 생성  
   <img width="533" alt="스크린샷 2024-12-20 오후 11 07 35" src="https://github.com/user-attachments/assets/36692611-11c9-4b75-b28c-5b9d24d449df" />

2. 버전명으로 태그 생성
