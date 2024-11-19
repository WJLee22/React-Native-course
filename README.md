# Installing Requirements  

<br>

## 1. expo-cli 설치

```
//at Windows PowerShell.
npm install --global expo-cli
```

<br>


## 2. 핸드폰 안드로이드 Play Store에서 Expo 다운로드 & 계정생성


![image](https://github.com/user-attachments/assets/292b942b-0c9f-4b7a-ad48-73657e860362)

<br>

## 3. Expo 프로젝트 생성 & Expo 로그인(Expo계정 이메일 or 닉네임)

```
npx create-expo-app 앱이름 --template  //Expo 프로젝트 생성// (입력후 뜨는 리스트에서 -> `blank` 선택하기)
or => npx create-expo-app (생성할 프로젝트 이름) --template blank    
npx expo login   //Expo 로그인// (입력후, Expo 가입할때 작성했던 이메일(or 닉네임) 입력 → 비밀번호 입력)
```

<br>

> + npx expo login 으로 pc에서 로그인해주고 + 폰에서도 Expo앱 접속중이어야함.  
> + expo init -> `npx create-expo-app --template`으로 명령어가 변경됨.  
> + expo login => `npx expo login`으로 명령어가 변경됨.  
> + 주의) powershell 에서는 불가능  



<br>

> + Expo를 이용하면 별도의 complie -> App 생성 과정x  
> + Expo를 이용하여, 우리가 만드는 React Native 소스코드를 곧바로 폰으로 전송  
> + Expo는 폰 안에 있는 React Native 소스코드를 실행시킴 -> 폰에서 React Native코드를 바로 미리보기 가능
> + 우리가 해야하는건 그저 JavaScript & Markup/Styling 코드를 작성-변경시키는 것 뿐, 나머지는 Expo에서 해줌

<br>

## 4. Expo 프로젝트 실행

```
npx start  or  npx expo start
```
<br>

### 4-1. -w 옵션으로 웹에서도 프로젝트를 실행하고싶을때!
웹에서도 프로젝트를 실행하기 위해서는 종속성을 따로 설치해줘야 함.
```
npx expo install react-dom react-native-web @expo/metro-runtime
```

<br>

### 4-2. -a 옵션으로 안드로이드 스튜디오 에뮬레이터 자동 실행 & Expo구동시키는 법!

<br>

> 안드로이드 스튜디오 에뮬레이터를 실행시키고 -> 이 에뮬레이터에 Expo 앱을 자동으로 설치하고 실행되도록 해볼 수 있다.
> 
> 매번 QR코드 찍어서 폰으로 확인 or 매번 안드로이드 스튜디오 들어가서 에뮬레이터 켜놓고 대기하기 => `이건 너무 귀찮으니깐.. 자동화시키자`  

<br>

1. Android Studio 를 실행하고, 메뉴에서 Customize 클릭 후 All settings..를 클릭
   
2. 좌측 상단의 검색창에 Android SDK를 검색하여 클릭한 후 Android SDK Location을 복사
   
3. 윈도우 검색창에 시스템 환경 변수 편집을 클릭
   
4. 우측 하단의 환경 변수버튼 클릭
   
5. 시스템 변수칸의 새로만들기를 클릭하여 아래의 값을 입력
```
변수 이름: ANDROID_HOME
변수 값: 2단계에서 복사해둔 sdk 주소(Android SDK Location)
```
6. 시스템 변수 리스트 중에서 `path`를 클릭 -> 편집버튼 클릭 -> 새로만들기 클릭 -> 아래의 값을 추가
```
%ANDROID_HOME%\platform-tools
```
  **7. cmd를 실행하고 아래의 명령어를 입력**
```
%ANDROID_HOME%\emulator\emulator -avd [AVD 이름]
```
8. Android Studio 에뮬레이터가 실행된 모습확인

9. VSCode 프로젝트 디렉터리 터미널로 돌아와서 `npx expo start` 및 `npm start`로 expo 를 실행    
 
10. `a 키 입력` -> 7단계에서 설정해둔 에뮬레이터가 실행되어지고, 이 에뮬에 Expo 앱이 자동으로 설치되고 실행되어짐    




<br><br><hr><br>

## 📱 React-Native앱의 전체 구조

<div align="center"><img src="https://github.com/user-attachments/assets/9ef1ebdb-613e-4a52-ad5f-e16195b63596"></div>


<br><br><br><br>
