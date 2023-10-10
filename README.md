# DataStructure

## 자료구조

## 시간복잡도
- 빅 오 표기법(big-O notation): 자료구조, 알고리즘 성능을 표시하기 위함
  > 빅오(Big-O), 빅세타(big-Θ), 빅오메가(big-Ω)

- 예시
  > [1, 2, 3, 4, 5] 배열이 있습니다. <br>
  > '3번째 숫자'를 찾을 경우 => 작업량 1 <br>
  > '숫자 4'를 찾을 경우 => 왼쪽에서부터 1234 작업량 4 <br>
  > 지금은 12345가 순서대로 있지만 4가 맨 앞에 있을 경우 작업량 1 / 맨 마지막에 있을 경우 작업량 5 <br>
  > 어떤 자료구조에 데이터가 얼마나 있을지 모르기 때문에 데이터의 총 개수를 n으로 표시하면 <br>
  > 어떤 값을 찾는 작업량을 n으로 표시할 수 있다. <br>
  > 데이터가 n개인 배열에서 특정 자리를 찾는 것은 1, 특정 값을 찾는 것은 n

- 빅오(Big-O)는 최악의 경우, 빅오메가(big-Ω)는 최선의 경우, 빅세타(big-Θ)는 최악과 최선이 같을 때

- 최악의 경우 작업량이 엄청나게 늘어나는 경우가 있기 때문에 보통 최악의 경우를 잘 고려해야 한다

- 대략 O(1), O(log n), O(n), O(nlog n), O(n^2), O(n^3), O(n^n), O(n!)의 순서대로 알고리즘이 점점 비효율적이 된다.

- 최악의 경우(Big-O)는 최선의 알고리즘을 사용했음에도 최악인 경우를 말한다.

- 업다운 게임 예시
  > 1부터 100중에 49를 찾는다고 가정합니다 <br>
  > 50 다운, 25 업, 37 업, 43 업, 46 업, 48 업, 49 => 총 7번 <br>
  > 이렇게 절반씩 줄여가면서 찾을 경우 => O(log n) <br>
  > 만약 1부터48까지, 50부터100까지 다 부르고 마지막에 49를 찾을 경우 => O(n) <br>

- for문 예시 <br>
  > for (let i = 0; i < arr.length; i++)에서 0부터 배열의 길이까지 반복하므로 => O(n) <br>
  > 이중 for문에서는 => O(n^2), 반복문이 3번있으면 O(n^3) ... <br>
  > for (let i = 0; i < arr.length; **i * 2**)에서 i가 배로 늘어나면 보통 O(log n) <br>
  > 이중 for문에서 순차적으로 늘어나는 것과 배로 늘어나는 것이 있으면 O(nlog n) <br>

## 공간복잡도
