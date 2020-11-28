# Problem

대문자와 소문자가 섞여있는 문자열 s가 주어집니다.

s에 'p'의 개수와 'y'의 개수를 비교해 같으면 True,

다르면 False를 return 하는 solution를 완성하세요.

'p', 'y' 모두 하나도 없는 경우는 항상 True를 리턴합니다.

단, 개수를 비교할 때 대문자와 소문자는 구별하지 않습니다.

예를 들어 s가 pPoooyY면 true를 return하고 Pyy라면 false를 return합니다.

## 제한 사항

- 문자열 s의 길이 : 50 이하의 자연수
- 문자열 s는 알파벳으로만 이루어져 있습니다.

## 입출력 예시


<img width="467" alt="mers1" src="https://user-images.githubusercontent.com/67893516/100522612-c78f4e80-31ed-11eb-8d80-aea5a39e6f77.png">

# 해결 방법

입력받은 문자열 s를 전부 소문자로 바꿔주고 split을 이용해 한 문자로 구분했다

그리고 fileter함수를 이용해서 v가 p거나 y인것만 담아주고

count와 count2 변수를 선언했다

filter함수로 p와 y만 담긴 배열을 for문을 통해 순회하면서

fil[i]가 'p'와 일치하면 count를 올려주고

fil[i]가 'y'와 일치하면 count2를 올려주었다

그리고 count와 count2의 수가 같은지를 리턴했다

count와 count2가 같다는 것은 p와 y의 개수가 일치한다는 얘기고

같지 않다면 false를 리턴할 것이라고 생각했다

좀 복잡하게 풀었다. 더 쉬운 방법이 있을 것 같은데

# 코드 구현

![mers2](https://user-images.githubusercontent.com/67893516/100522614-c8c07b80-31ed-11eb-80eb-2998b153d918.png)

# 실행 결과

<img width="605" alt="mers3" src="https://user-images.githubusercontent.com/67893516/100522618-ca8a3f00-31ed-11eb-9ff9-6bf0f8aab73a.png">

# 다른 사람의 풀이

![mers4](https://user-images.githubusercontent.com/67893516/100522621-ce1dc600-31ed-11eb-9a1c-23afc06cc15e.png)

역시 내가 문제를 해결하고 다른 사람의 풀이를 보면 배우는 게 참 많다

나 역시 소문자 혹은 대문자로 바꾸고 split으로 문자를 구분해주었지만

구분 기준을 'P'나 'Y'로 할 생각은 못했다

그리고 구분시킨 문자열의 길이를 비교해서 리턴하다니

오늘도 하나 배웠다.