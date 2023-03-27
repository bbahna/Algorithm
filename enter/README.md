# Algorithm study
## enter 입문(100문제): [JavaScript, Lv.0](https://school.programmers.co.kr/learn/challenges/beginner?order=acceptance_desc&languages=javascript)

### Day 1 사칙연산
1. 두 수의 합
    ```
    function solution(num1, num2) {
      var answer = num1+num2;
      return answer;
    }
    ```
2. 두 수의 차
    ```
    function solution(num1, num2) {
        var answer = num1 - num2;
        return answer;
    }
    ```
3. 두 수의 곱
    ```
    function solution(num1, num2) {
        var answer = num1 * num2;
        return answer;
    }
    ```
4. 몫 구하기
    ```
    function solution(num1, num2) {
        var answer = parseInt(num1 / num2);
        return answer;
    }
    ```

### Day 2 사칙연산, 조건문, 배열
5. 두 수의 나눗셈
    ```
    function solution(num1, num2) {
        const answer = parseInt((num1/num2)*1000);
        return answer;
    }
    ```
6. 숫자 비교하기
    ```
    function solution(num1, num2) {
        if(num1 == num2) {
            return 1;
        } else{
            return -1;
        }
    }
    ```
7. 분수의 덧셈
    ```

    ```
8. 배열 두 배 만들기
    ```
    function solution(numbers) {
        const answer = numbers.map((item)=>{
            return item*2;
        })
        return answer;
    }
    ```