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

### Day 3 사칙연산, 배열, 수학
9. 나머지 구하기
    ```
    function solution(num1, num2) {
        const answer = num1%num2;
        return answer;
    }
    ```
10. 중앙값 구하기
    ```
    function solution(array) {
        const sortArray = array.sort((a, b) =>{
            return a - b;
        })

        const answer = sortArray[Math.floor(array.length / 2)];
        return answer;
    }
    ```
11. 최빈값 구하기
    ```

    ```
12. 짝수는 싫어요
    ```
    function solution(n) {
        let even = (n % 2 == 1) ? Math.floor(n/2 + 1) : n/2;

        const answer = Array(even).fill().map((v,i) => 2 * i + 1);
        return answer;
    }
    ```

### Day 4 수학, 배열
13. 피자 나눠 먹기 (1)
    ```
    function solution(n) {
        const answer = Math.ceil(n/7);
        return answer;
    }
    ```
14. 피자 나눠 먹기 (2)
    ```

    ```
15. 피자 나눠 먹기 (3)
    ```
    function solution(slice, n) {
        const answer = Math.ceil(n / slice);
        return answer;
    }
    ```
16. 배열의 평균값
    ```
    function solution(numbers) {
        const numberSum = numbers.reduce((a,b) => (a+b));

        const answer = numberSum/numbers.length
        return answer;
    }
    ```