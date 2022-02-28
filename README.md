# 정규표현식

정규식, Regular Expression

## 역할

- 문자 검색(search)
- 문자 대체(replace)
- 문자 추출(extract)

## 테스트 사이트

https://regexr.com/

## 정규식 생성

```JS
// 생성자 방식
new RegExp('표현', '옵션')
new RegExp('[a-z]', 'gi') // a-z까지의 영어 소문자를 검색하는 표현.
//gi는 대소문자 구분 없이 일치하는 모든 결과를 검색하겠다는 옵션

// 리터럴 방식
/표현/옵션
/[a-z]/gi
```

## 예제 문자

```JS
const str = `
010-1234-5679
oxywriter@gmail.com
http://www.omdbapi.com/?apikey=7035c60c&s=frozen
The quick brown fox jumps over the lazy dog.
asdjnfakasdkfhfh
`
```

## 메소드

메소드 | 문법 | 설면
--|--|--
test | `정규식.test(문자열)` | 일치 여부(Boolean) 반환
match | `문자열.match(정규식)` | 일치하는 문자의 배열(Array) 반환
replace | `문자열.replace(정규식, 대체문자)` | 일치하는 문자를 대체