---
## title: 프로그래머스 완주하지 못한 선수
author: Choi eun ji
date: 2020-09-02 14:00:00 +0800
categories: [Blogging, algorithm]
tags: [programmars,java]
pin: true
---

## 완주하지 못한 선수(programmars)

programmars 문제풀이를 level 1부터 시작한다. 머리굴리기 싫어....

일단 문제내용을 간략히 정리해보면

##### 문제 설명
수많은 마라톤 선수들이 마라톤에 참여하였습니다. 단 한 명의 선수를 제외하고는 모든 선수가 마라톤을 완주하였습니다.

마라톤에 참여한 선수들의 이름이 담긴 배열 participant와 완주한 선수들의 이름이 담긴 배열 completion이 주어질 때, 완주하지 못한 선수의 이름을 return 하도록 solution 함수를 작성해주세요.

##### 제한사항
1. 마라톤 경기에 참여한 선수의 수는 1명 이상 100,000명 이하입니다.
2. completion의 길이는 participant의 길이보다 1 작습니다.
3. 참가자의 이름은 1개 이상 20개 이하의 알파벳 소문자로 이루어져 있습니다.
4. 참가자 중에는 동명이인이 있을 수 있습니다.

이와 같은 내용인데 생각해보면 간단하다. 그냥 다 비교해보고 없는사람 하나 찾으면 되는거 아니야?  
..물론 그러면 비효율적이다.

```java
import java.util.Arrays;

class Solution {
    public String solution(String[] participant, String[] completion) {
        String answer = "";
        int i=0;
        Arrays.sort(participant);
        Arrays.sort(completion);
      for(i=0;i<completion.length;i++)
      {
          if(!participant[i].equals(completion[i]))
          {
             return participant[i];
          }
      }
        return participant[i];
    }
}
```
결국에 통과한코드
정렬을 한뒤 비교한다.

### 오늘의 교훈
어떤 문제던 종이, 펜과 함께하자.
