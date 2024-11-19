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

### 4-1. -w 옵션으로 웹에서도 프로젝트를 실행하고싶을때!
웹에서도 프로젝트를 실행하기 위해서는 종속성을 따로 설치해줘야 함.
```
npx expo install react-dom react-native-web @expo/metro-runtime
```


<br><br><hr><br>

## 📱 React-Native앱의 전체 구조

<div align="center"><img src="https://github.com/user-attachments/assets/9ef1ebdb-613e-4a52-ad5f-e16195b63596"></div>


<br><br><br><br>
