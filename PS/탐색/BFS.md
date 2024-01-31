# 그래프 완전 탐색

## BFS (Breadth-First Search)

> 그래프의 시작 노드에서 출발해 시작 노드를 기준으로 **가까운 노드를 먼저 방문하면서 탐색**하는 알고리즘.

> [여담] 드라마를 1화씩만 여러개 보는 타입

```
void BFS(int k) {
  queue<int> q;v
  q.push(k);
  visited[k] = true;

  while(!q.empty()) {
    int now = q.front();
    q.pop();
    cout << now << ' ';

    for(int i: graph[now]) {
      if(!visited[i]) {
        visited[i] = true;
        q.push(i);
      }
    }
  }
}
```

## 관련 문제

- [[Gold II] 트리의 지름 - 1167](https://github.com/jeongwoo903/coding-test/tree/main/%EB%B0%B1%EC%A4%80/Gold/1167.%E2%80%85%ED%8A%B8%EB%A6%AC%EC%9D%98%E2%80%85%EC%A7%80%EB%A6%84)
- [[Silver II] DFS와 BFS - 1260](https://github.com/jeongwoo903/coding-test/tree/main/%EB%B0%B1%EC%A4%80/Silver/1260.%E2%80%85DFS%EC%99%80%E2%80%85BFS)
