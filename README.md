<!-- Heading -->
# MeTA9`s Library
![image](https://github.com/user-attachments/assets/e1d2d0fb-e160-4554-9a68-94f6ccea70a3)


## 기본세팅
```lua
loadstring(game:HttpGet("https://raw.githubusercontent.com/META9999/MeTA9-Library/refs/heads/main/main.lua"))()
```
코드 해석 : main.lua의 코드를 불러옵니다



## 창 만들기
```lua
local window = Library:CreateWindow("ㅇㅈ")
```
코드 해석 : Library 테이블 안에 있는 매서드인 CreatWindow 매서드로 창을 만듭니다. ()안에 있는 문자열은 창의 이름입니다

## 탭 만들기
```lua
local tab = window:CreateTab("Tab")
```
코드 해석 : Library 테이블 안에 있는 매서드인 CreatTab 매서드로 창을 만듭니다.

## 버튼 만들기
```lua
tab:AddButton("Button", "설명", function()
    print("Button Pressed")
end)
```
코드 해석 : AddButton매서드로 버튼을 만듭니다. 첫번째 문자열은 버튼의 이름, 두번째 문자열은 설명입니다. 안에 있는 코드는 버튼을 눌렀을때 실행하는 코드입니다.


## 슬라이드 만들기

```lua
tab:AddSlider("Slider", "0부터 100까지 값을 조절할 수 있는 슬라이더입니다.", 0, 100, 50, function(value)
    print("Slider Value:", value)
end)
```
코드 해석 : 4번째 숫자는 최소값, 5번째는 최대값, 6번째는 기본값입니다.


## 체크박스 만들기

```lua
tab:AddToggle("Toggle", "켜기/끄기를 전환할 수 있는 토글 버튼입니다.", false, function(value)
    print("Toggle Value:", value)
end)
```
코드  해석 : 두번째 값은 기본값입니다.

## 알림창 만들기

```lua
tab:Notify("Welcome!", "MeTA9's Library에 오신 것을 환영합니다!", 3)
```

코드 해석 : 3번째 값은 창을 유지하는 시간입니다.

