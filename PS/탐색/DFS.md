# 그래프 완전 탐색

## 대표적 문제 유형

1. 경로탐색 유형(최단 거리)
2. 네트워크 유형(연결)
3. 조합 유형(모든 조합 만들기, 경우의 수)

## DFS (Depth-First Search)

> 그래프의 시작 노드에서 출발하여 탐색할 한쪽 분기를 정하여 **최대 깊이 까지 탐색**을 마친 후, 다른 쪽 분기로 이동하여 다시 탐색을 수행하는 알고리즘.

> [여담] 드라마를 한 번 꽃히면 몰아서 보는 유형

```
void DFS(int k) {
  if(visited[k]) { return; }
  visited[k] = true;
  cout << k << ' ';

  for(int i: graph[k]) {
    if(!visited[i]) { DFS(i); }
  }
}
```

## 관련 문제

- [[Gold V] 신기한 소수 - 2023](https://github.com/jeongwoo903/coding-test/blob/main/%EB%B0%B1%EC%A4%80/Gold/2023.%E2%80%85%EC%8B%A0%EA%B8%B0%ED%95%9C%E2%80%85%EC%86%8C%EC%88%98/README.md)
- [[Silver II] 연결 요소의 개수 - 11724](https://github.com/jeongwoo903/coding-test/tree/main/%EB%B0%B1%EC%A4%80/Silver/11724.%E2%80%85%EC%97%B0%EA%B2%B0%E2%80%85%EC%9A%94%EC%86%8C%EC%9D%98%E2%80%85%EA%B0%9C%EC%88%98#silver-ii-%EC%97%B0%EA%B2%B0-%EC%9A%94%EC%86%8C%EC%9D%98-%EA%B0%9C%EC%88%98---11724)
- [[Gold V] ABCDE - 13023](https://github.com/jeongwoo903/coding-test/blob/main/%EB%B0%B1%EC%A4%80/Gold/13023.%E2%80%85ABCDE/README.md)
