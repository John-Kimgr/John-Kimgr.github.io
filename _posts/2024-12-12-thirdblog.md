---
title: "[Markdown]문서 작성하기"
description: Markdown을 활용한 문서작성 방법
date: 2024-12-12 20:21:00 +0900
categories: [Markdown]
tags: [markdown, tutorial]
pin: true
math: false
mermaid: false
---


## Markdown이란?
Markdown은 **텍스트 기반 문서 작성 언어**로, 간단한 문법을 통해 텍스트를 구조화하고 포맷팅할수 있는 언어다.<br>
Github에서 README 파일 작성과 프로젝트 문서화를 위해 필수적으로 사용된다.<br>
Markdown을 잘 이해하고 활용하면 깔끔하고 읽기 쉬운 문서 작성이 가능하며, 협업 시 효과적인 정보전달이 가능하다.


---

### **1. 헤더 (Headers)**
헤더는 문서의 제목과 섹션을 구분하는 데 사용되는데, #의 갯수에 증가함에 따라 글자의 크기가 작아짐.

```bash
# 제목 1
## 제목 2
### 제목 3
#### 제목 4
##### 제목 5
###### 제목 6
```
## **결과**
# 제목 1
## 제목 2
### 제목 3
#### 제목 4
##### 제목 5
###### 제목 6

---

### **2. 텍스트 스타일(Text Style)**
```bash
**굵게**
*기울임체*
~~취소선~~
`코드 강조`
```
**결과:**<br>
**굵게**<br>
*기울임체*<br>
~~취소선~~<br>
`코드 강조`<br>

---

### **3. 리스트(List)**
순서가 있는 리스트와 없는 리스트 작성이 가능하다.<br>
**순서가 없는 리스트:**
```bash
- 항목 1
- 항목 2
    - 하위 항목 1
    - 하위 항목 2
```
**결과**
- 항목 1
- 항목 2
    - 하위 항목 1
    - 하위 항목 2

**순서가 있는 리스트:**
```bash
1. 첫 번째
2. 두 번째
3. 세 번째
```
**결과**
1. 첫 번째
2. 두 번째
3. 세 번째

---
### **4. 링크와 이미지 **
**링크 추가:**
```bash
[Link Test](https://john-kimgr.github.io/)
```
**결과:** [Link Test](https://john-kimgr.github.io/)

**이미지추가:**
```bash
![Markdown symbol](https://markdown-here.com/img/icon256.png)
```
**결과**<br>
![Markdown symbol](https://markdown-here.com/img/icon256.png)

---

### **5.코드 블록**
**인라인 코드**
```bash
`인라인 코드 테스트`
```
**결과:** `인라인 코드 테스트`
<br>

**여러 줄 코드:**
```bash
```python
def hello_world():
    print("Hello, World!")
```
**결과:**
```python
def hello_world():
    print("Hello, World!")
```

---
### **6.테이블**
테이블을 사용하여 간단한 표를 작성할 수 있다.<br>
```bash
| 제목 1   | 제목 2   |
|----------|----------|
| 내용 1   | 내용 2   |
| 내용 3   | 내용 4   |
```
**결과:**

| 제목 1   | 제목 2   |
|---------|---------|
| 내용 1   | 내용 2   |
| 내용 3   | 내용 4   |
| 내용 3   | 내용 4   |

- css 설정에서 뭔가 문제가 있었는지 색상 문제가 조금 있습니다. 
- 왼쪽 사이드바 하단 모드 변경을 눌러 다크모드로 보면 문제 없습니다

---
### **7.배지**
```bash
![Build Status](https://img.shields.io/badge/build-passing-brightgreen)
```
**결과:**
![Build Status](https://img.shields.io/badge/build-passing-brightgreen)

---

## **결론**
위와 같이 다양한 방법으로 문서를 작성하면, 텍스트로만 가득 채운 것 보다 훨씬 가독성이 좋을 것 같다.
조금 더 능숙해 질 수 있또록 지속적으로 포스팅하는 연습을 해야 할 것 같다.