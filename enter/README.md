# Algorithm study
## enter 입문(100문제): [programmers, Lv.0](https://school.programmers.co.kr/learn/challenges/beginner?order=acceptance_desc&languages=javascript)

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

### Day 5 수학, 배열
17. 옷가게 할인 받기
    ```
    function solution(price) {
        const 십만원 = 100000;
        
        if (price >= 십만원*5) {
            return Math.floor(price*0.8);
        } else if (price >= 십만원*3) {
            return Math.floor(price*0.9);
        } else if (price >= 십만원) {
            return Math.floor(price*0.95);
        } else {
            return price
        }
    }
    ```
18. 아이스 아메리카노
    ```
    function solution(money) {    
        return [Math.floor(money/5500), money%5500];
    }
    ```
19. 나이 출력
    ```
    function solution(age) {
        return new Date().getFullYear() - age + 1;
    }
    ```
20. 배열 뒤집기
    ```
    function solution(num_list) {
        return num_list.reverse()
    }
    ```

### Day 6 문자열, 반복문, 출력, 배열, 조건문
21. 문자열 뒤집기
    ```
    function solution(my_string) {
        return my_string.split('').reverse().join('');
    }
    ```
22. 직각삼각형 출력하기
    ```

    ```
24. 짝수 홀수 개수
    ```
    function solution(num_list) {
        let even = 0;
        let odd = 0;

        for(let i=0; i < num_list.length; i++) {
            if(num_list[i]%2 == 0)  {
                even++;
            } else {
                odd++;
            }
        }

        return [even, odd];
    }
    ```
24. 문자 반복 출력하기
    ```
    function solution(my_string, n) {    
        return [...my_string].map(i => i.repeat(n)).join('')
    }
    ```
    
### Day 7 문자열, 반복문, 출력, 배열, 조건문
26. 특정 문자 제거하기
    ```
    
    ```

27. 각도기
    ```
    
    ```

28. 양꼬치
    ```
    
    ```

29. 짝수의 합
    ```
    
    ```

### Day 8 배열, 구현, 수학
30. 문제명
    ```
    
    ```

31. 문제명
    ```
    
    ```

32. 문제명
    ```
    
    ```

33. 문제명
    ```
    
    ```

### Day 9 수학, 문자열, 해시, 완전탐색, 조건문
34. 문제명
    ```
    
    ```

35. 문제명
    ```
    
    ```

36. 문제명
    ```
    
    ```

37. 문제명
    ```
    
    ```

### Day 10 조건문, 배열, 수학, 시뮬레이션
38. 문제명
    ```
    
    ```

39. 문제명
    ```
    
    ```

40. 문제명
    ```
    
    ```

41. 문제명
    ```
    
    ```

### Day 11 수학, 반복문
42. 문제명
    ```
    
    ```

43. 문제명
    ```
    
    ```

44. 문제명
    ```
    
    ```

45. 문제명
    ```
    
    ```

### Day 12 문자열, 정렬, 사칙연산, 수학
46. 문제명
    ```
    
    ```

47. 문제명
    ```
    
    ```

48. 문제명
    ```
    
    ```

49. 문제명
    ```
    
    ```

### Day 13 문자열, 배열, 사칙연산, 수학, 조건문
50. 문제명
    ```
    
    ```

51. 문제명
    ```
    
    ```

52. 문제명
    ```
    
    ```

### Day 14 조건문, 반복문, 시뮬레이션, 문자열
53. 문제명
    ```
    
    ```

54. 문제명
    ```
    
    ```

55. 문제명
    ```
    
    ```

56. 문제명
    ```
    
    ```

### Day 15 문자열, 해시, 배열, 수학
57. 문제명
    ```
    
    ```

58. 문제명
    ```
    
    ```

59. 문제명
    ```
    
    ```

60. 문제명
    ```
    
    ```

### Day 16 문자열, 수학, 배열, 조건문
61. 문제명
    ```
    
    ```

62. 문제명
    ```
    
    ```

63. 문제명
    ```
    
    ```

64. 문제명
    ```
    
    ```

### Day 17 문자열, 수학, 조건문, 배열, 사칙연산
65. 문제명
    ```
    
    ```

66. 문제명
    ```
    
    ```

67. 문제명
    ```
    
    ```

68. 문제명
    ```
    
    ```

### Day 18 문자열, 수학, 조건문, 정렬
69. 문제명
    ```
    
    ```

70. 문제명
    ```
    
    ```

71. 문제명
    ```
    
    ```

72. 문제명
    ```
    
    ```

### Day 19 문자열, 배열, 조건문
73. 문제명
    ```
    
    ```

74. 문제명
    ```
    
    ```

75. 문제명
    ```
    
    ```

76. 문제명
    ```
    
    ```

### Day 20 수학, 시뮬레이션, 문자열, 사칙연산
77. 문제명
    ```
    
    ```

78. 문제명
    ```
    
    ```

79. 문제명
    ```
    
    ```

80. 문제명
    ```
    
    ```

### Day 21 문자열, 사칙연산, 시뮬레이션, 2차원배열, 수학, 배열
81. 문제명
    ```
    
    ```

82. 문제명
    ```
    
    ```

83. 문제명
    ```
    
    ```

84. 문제명
    ```
    
    ```

### Day 22 dp, 수학, 조건문, 배열
85. 문제명
    ```
    
    ```

86. 문제명
    ```
    
    ```

87. 문제명
    ```
    
    ```

88. 문제명
    ```
    
    ```

### Day 23 배열, 정렬, 문자열
89. 문제명
    ```
    
    ```

90. 문제명
    ```
    
    ```

91. 문제명
    ```
    
    ```

92. 문제명
    ```
    
    ```

### Day 24 수학, 시뮬레이션, 문자열, 조건문, 반복문
93. 문제명
    ```
    
    ```

94. 문제명
    ```
    
    ```

95. 문제명
    ```
    
    ```

96. 문제명
    ```
    
    ```

### Day 25 시뮬레이션, 조건문, 수학
97. 문제명
    ```
    
    ```

98. 문제명
    ```
    
    ```

99. 문제명
    ```
    
    ```

100. 문제명
        ```
        function solution() {
            const answer = 0;
            return answer;
        }
        ```