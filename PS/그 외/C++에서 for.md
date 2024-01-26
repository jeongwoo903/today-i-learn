# C++에서 python과 같이 for문 쓰기

## 배열 안에 들어있는 값만 꺼내서 for 돌리기

```
  int n_list[4] = {1,3,7,9};

  for(int i: n_list) {
    int x = num * 10 + i;
    if(isPrime(x)) { DFS(x, digit + 1); }
  }
```

소수 문제를 풀다가 알게 되었는데 꽤나 유용하다.  
다만 string에 대해서는 auto를 써주어야 한다.
