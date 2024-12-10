---
title: "[Jekyll] GitHub Pages 만들기"
description: Jekyll-theme-chirpy를 이용한 블로그 작성
date: 2024-12-04 00:34:00 +0900
categories: [Tutorial]
tags: [jekyll, chirpy, github-pages]
pin: true
math: false
mermaid: false
---

# 도입 
### Jekyll의 **Chirpy** 테마를 이용하여 블로그를 만드는 작업을 기록하려고 합니다.

---

## 1. GitHub Pages Repository 생성
1. [GitHub](https://github.com)에 접속하여 새로운 레포지토리를 생성
   - 레포지토리명: `[사용할 username].github.io`
   - 공개범위를 **Public**으로 설정하고, 초기화 시 `README.md`를 추가

---

## 2. Chirpy 테마 복제
Chirpy 테마는 GitHub 레포지토리로 제공되므로, 로컬 환경으로 clone

```bash
git clone https://github.com/cotes2020/jekyll-theme-chirpy.git
```

복제한 디렉토리로 이동
```bash
cd /폴더경로/jekyll-theme-chirpy
```

---

## 3. 레포지토리 연결
복제한 Chirpy 테마를 GitHub Pages 레포지토리와 연결

```bash
git remote set-url origin https://github.com/[username]/[username].github.io.git
```

---

## 4. 로컬 환경을 위한 설치 및 테스트

1. Ruby 설치:
- Windows: RubyInstaller를 사용하여 설치
- MacOS : `brew install ruby`
- Linux : `sudo apt install ruby-full`

2. Bundler 설치
```bash
gem install jekyll bundler
gem install webrick
```

3. Jekyll 생성
```bash
jekyll new ./
```

4. bundle 설치
```bash
bundle install
```

5. Jekyll 서버 작동 확인
```bash
bundle exec jekyll serve
```

6. 로컬 테스트
- <http://127.0.0.1:4000/>또는 <http://localhost:4000/>로 접속하여 확인

## 5. GitHub에 Push
변경된 내용을 GitHub에 push하여 배포
```bash
git add .
git commit -m "chirpy theme"
git push origin main
```

## 6. pages 활성화
1. 레포지토리의 Settings 이동
2. pages 메뉴로 이동후
3. Build and deployment에서 Source를 GitHub Actions로 변경
4. 변경 이유는 Deploy from a branch로 할 경우 활성화되지 않을 수 있음


## 7. 배포 확인
1. push 후 즉시 반영되는 것이 아니기 때문에 5~10분정도 후 해당 주소에 접속하여 확인
2. 이 페이지의 경우 주소는 <https://john-kimgr.github.io/>