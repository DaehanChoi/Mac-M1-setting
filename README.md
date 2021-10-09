## Mac-M1-setting
# pyenv 버젼 관리시 생기는 문제 해결법
1. xcode 설치 및 경로 설정
2. pyenv 및 pyenv-virtualenv 설치
```
brew install pyenv pyenv-virtualenv
```
>아래의 과정을 거치지않으면 
>BUILD FAILED (OS X 11.4 using python-build 20180424) 에러 발생

3. 경로설정
```
 vim ~/.zshrc
 #내용 추가
 export PATH="$HOME/.pyenv/bin:$PATH"
 eval "$(pyenv init -)"
 eval "$(pyenv virtualenv-init -)"
 pyenv install 3.8.6
```
4.
