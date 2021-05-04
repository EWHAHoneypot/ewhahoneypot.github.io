# 2021 EWHA Cyber Security 졸업 프로젝트 Technical Log (Deeplearning, Kotlin, Django, Go-Gin, AWS, Docker, K8S)
## 환경 구축
### 1. 템플릿 Clone
#### 적당한 템플릿을 github.io 로컬 저장소에 다운로드한다.

### 2. Ruby Download & _config.yml
#### https://rubyinstaller.org/ 에서 다운로드 및 설치
```
$ ruby -v
$ gem install jekyll bundler
```
#### 잘 설치되었는지 확인 (ruby version 확인) & Jekyll, Bundler 설치
#### _config.yml 파일을 다음과 같이 수정
```yml
url : "https://yourusername.github.io"
baseurl : "" # 공백으로 해도 무방, 혹은 /blog, /gitblog 등

remote_theme : arnp/herring-cove # 사용하는 템플릿에 맞게 수정
```


### 3. Gemfile 수정 & 로컬에서 구동
#### Gemfile이 없는 경우 ```$bundle init``` 으로 생성 후 Gemfile에 다음 입력
``` ruby
git_source(:github) {|repo_name| "https://github.com/username.github.io" }

gem "jekyll", "~> 4.2.0"

gem 'wdm', '>= 0.1.1'
```
