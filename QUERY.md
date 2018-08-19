# QUERY
### 문제 설명
N개의 원소를 가진 배열 A가 주어진다.

당신은 Q개의 쿼리를 처리하여야 한다.

    Query(i, j, k) : A[i ... j] 중 k 이하인 원소의 갯수
배열 A와 Q개의 쿼리에 대해 i, j, k가 주어질 때 Query(i, j, k) 값을 출력하시오.
### 입력
첫째 줄에 N과 Q가 주어진다. (1 <= N, Q <= 10^5)

둘째 줄에 A[1 ... N]이 주어진다. (1 <= A[i] <= 10^9)

셋째 줄부터 Q개의 줄에 대해 i, j, k가 주어진다. (1 <= i, j <= N) (1 <= k <= 10^9)
### 출력
Q개의 쿼리에 대해 Query(i, j, k) 값을 출력한다.
### Solution
- <code>Merge Sort Tree</code>와 <code>upper_bound</code>를 이용하여 O(N lg^2 N)의 시간복잡도로 해결 가능하다.
- <code>Persistent Segment Tree</code>를 이용해 <code>A[1...j] 중 k 이하인 원소의 갯수 - A[1 ... i - 1] 중 k 이하인 원소의 갯수</code>를 O(lg N)의 시간복잡도로 구할 수 있다. 단 A[i] 값이 크므로 좌표압축을 해야한다.
- <code>Sqrt Decomposition</code>을 이용해 O(Q sqrt(N))의 시간복잡도로 해결할 수 있다.
