# Algorithm study
## kit 고득점 - [programmers, 코딩테스트 자주 나오는 유형](https://school.programmers.co.kr/learn/challenges?tab=algorithm_practice_kit)(10유형)

### 1. 정렬 - 알고리즘
`정렬을 이용해서 문제를 효율적으로 풀어보세요.`
> 출제빈도: 높음
>
> 평균점수: 높음
>
> 문제세트: 0 / 3

* K번째수(Lv.1) _230418
  ```
  function solution(array, commands) {
    let answer = [];

    for(let i=0; i < commands.length; i++) {
      const splicedArray = array.slice(commands[i][0] - 1, commands[i][1]);

      const sortedArray = splicedArray.sort((a, b) => a - b);

      answer.push(sortedArray[commands[i][2] - 1]);
    }

    return answer;
  }
  ```

* 가장 큰 수(Lv.2) _230419
  ```

  ```

* H-Index(Lv.2) _230419
  ```

  ```

### 2. 해시 - 자료구조
`Key-value쌍으로 데이터를 빠르게 찾아보세요.`
> 출제빈도: 높음
>
> 평균점수: 보통
>
> 문제세트: 0 / 5

* 폰켓몬(Lv. 1) _230419
  ```
  function solution(nums) {
    const 잡을수있음 = nums.length/2;
    const 중복값제거 = [...new Set(nums)].length;
    
    return 잡을수있음 < 중복값제거 ? 잡을수있음 : 중복값제거;
  }
  ```
 
* 완주하지 못한 선수(Lv. 1) _230419(풀이참고)
  ```
  function solution(participant, completion) {
    const participantSort = participant.sort();
    const completionSort = completion.sort();
    
    for(let i = 0; i < participantSort.length; i++) {
      if (participantSort[i] !== completion[i]) {
          return participantSort[i]
      }
    }
  }
  ```

* 전화번호 목록(Lv. 2) _js 미지원
  ```

  ```
 
* 위장(Lv. 2) _230420
  ```

  ```

* 베스트앨범(Lv. 3)
  ```

  ```

### 3. 완전탐색 - 알고리즘
`무식해 보여도 사실은 최고의 방법일 때가 있지요.`
> 출제빈도: 높음
>
> 평균점수: 낮음
>
> 문제세트: 0 / 7

* 최소직사각형(lv.1) _230424(아쉬운 코드..)
  ```
  function solution(sizes) {
    let sortSizes = [];

    for (let i = 0; i < sizes.length; i++) {
        sortSizes.push(sizes[i].sort((a, b) => b - a));
    }

    let sizesX = [];
    let sizesY = [];

    for (let i = 0; i < sortSizes.length; i++) {
        sizesX.push(sortSizes[i][0]);
    }

    for (let i = 0; i < sortSizes.length; i++) {
        sizesY.push(sortSizes[i][1]);
    }

    return Math.max(...sizesX)*Math.max(...sizesY);
  }
  ```
  
* 모의고사(lv.1) _230424
  ```

  ```

* 소수 찾기(lv.2)
  ```

  ```
  
* 카펫(lv.2)
  ```

  ```
  
* 피로도(lv.2)
  ```

  ```
  
* 전력망을 둘로 나누기(lv.2)
  ```

  ```
  
* 모음사전(lv.2)
  ```

  ```

### 4. 깊이/너비 우선 탐색(DFS/BFS) - 알고리즘
`깊이/너비 우선 탐색을 사용해 원하는 답을 찾아보세요.`
> 출제빈도: 높음
>
> 평균점수: 낮음
>
> 문제세트: 0 / 7

* 타겟 넘버(Lv. 2)
  ```
  ````
 
* 네트워크(Lv. 3)
  ```
  ````
 
* 게임 맵 최단거리(Lv. 2)
  ```
  ````
 
* 단어 변환(Lv. 3)
  ```
  ````
 
* 여행경로(Lv. 3)
  ```
  ````
 
* 아이템 줍기(Lv. 3)
  ```
  ````
 
* 퍼즐 조각 채우기(Lv. 3)
  ```
  ````

### 5. 스택/큐 - 자료구조
`LIFO, FIFO, push & pop! 스택과 큐를 이용해서 문제를 풀어보세요.`
> 출제빈도: 보통
>
> 평균점수: 높음
>
> 문제세트: 0 / 6

* 같은 숫자는 싫어(Lv. 1) _230424
  ```
  function solution(arr) {
      var answer = [];

      for (let i = 0; i < arr.length; i++) {
          if(arr[i] !==  arr[i+1]) {
              answer.push(arr[i])
          }
      }

      return answer;
  }
  ```

* 기능개발(Lv. 2) _230425
  ```
  ```
 
* 올바른 괄호(Lv. 2)
  ```
  ```
 
* 프로세스(Lv. 2)
  ```
  ```
 
* 다리를 지나는 트럭(Lv. 2)
  ```
  ```
 
* 주식가격(Lv. 2)
  ```
  ```

### 6. 힙(Heap) - 자료구조
`힙은 특정한 규칙을 가지는 트리로, 힙을 이용해서 우선순위 큐를 구현할 수 있습니다.`
> 출제빈도: 보통
>
> 평균점수: 높음
>
> 문제세트: 0 / 3

* 더 맵게(Lv. 2)
  ```
  ``` 
 
* 디스크 컨트롤러(Lv. 3)
  ```
  ``` 
 
* 이중우선순위큐(Lv. 3)
  ```
  ```

### 7. 탐욕법(Greedy) - 알고리즘
`부분적인 최적해가 전체적인 최적해가 되는 마법!`
> 출제빈도: 낮음
>
> 평균점수: 낮음
>
> 문제세트: 0 / 6

* 체육복(Lv. 1) _230425
  ```
  ```
 
* 조이스틱(Lv. 2)
  ```
  ```
 
* 큰 수 만들기(Lv. 2)
  ```
  ```
 
* 구명보트(Lv. 2)
  ```
  ``` 
 
* 섬 연결하기(Lv. 3)
  ```
  ```
 
* 단속카메라(Lv. 3)
  ```
  ```

### 8. 동적계획법(Dynamic Programming) - 알고리즘
`불필요한 계산을 줄이고, 효율적으로 최적해를 찾아야만 풀리는 문제들입니다.`
> 출제빈도: 낮음
>
> 평균점수: 낮음
>
> 문제세트: 0 / 5

* N으로 표현(Lv. 3)
  ```
  ``` 
 
* 정수 삼각형(Lv. 3)
  ```
  ``` 
 
* 등굣길(Lv. 3)
  ```
  ``` 
 
* 사칙연산(Lv. 4)
  ```
  ``` 
 
* 도둑질(Lv. 4)
  ```
  ```

### 9. 이분탐색 - 알고리즘
`이분탐색 기법을 이용해 효율적으로 값을 찾아보세요`
> 출제빈도: 낮음
>
> 평균점수: 낮음
>
> 문제세트: 0 / 2

* 입국심사(Lv. 3)
  ```
  ```
 
* 징검다리(Lv. 4)
  ```
  ```

### 10. 그래프 - 자료구조
`엣지를 지나 그래프의 노드를 탐험해봅시다.`
> 출제빈도: 낮음
>
> 평균점수: 낮음
>
> 문제세트: 0 / 3

* 가장 먼 노드(Lv. 3)
  ```
  ```
 
* 순위(Lv. 3)
  ```
  ```
 
* 방의 개수(Lv. 5)
  ```
  ```
