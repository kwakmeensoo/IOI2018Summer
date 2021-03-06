# THINKING HEAP
### 문제 설명
수업 시간에 O(lg N) 만에 삽입과 삭제가 가능한 자료구조인 Heap을 배운 민수는 Heap을 이용해 여러가지 숫자를 <code>PUSH</code>하고 <code>POP</code>한 결과, Heap에 <code>PUSH</code>한 순서에 따라 Heap의 내부에 저장되는 순서가 다르다는 걸 깨달았다.
Heap에 1 ~ N까지의 숫자를 <code>PUSH</code>할 때, i번째 정점에 K가 위치하도록 하는 <code>PUSH</code> 방법을 출력하시오.
### 입력
첫째 줄에, i(1 ≤ i ≤ N)와 K(1 ≤ K ≤ N)가 주어진다. Heap의 정점 번호는 1부터 시작한다고 가정한다.
### 출력
가능한 <code>PUSH</code> 방법 중, **아무거나 한 가지**를 출력하시오. 그러한 방법이 없다면 -1을 출력하시오.
### Solution
1번 정점부터 i번 정점의 부모정점까지의 경로를 1부터 채운 후, i번 정점의 자식정점들을 K + 1부터 채운다. 숫자가 부족하지 않고, 잘 채워졌다면 아직 채워지지 않은 정점들은 아직 채워지지 않은 숫자들로 순서대로 채운다. 정점을 모두 채웠으면 1번 정점부터 채워진 숫자로 <code>PUSH</code>하면 된다. 위의 방법대로 채웠다면, <code>PUSH</code>한 후 업데이트가 되지 않으므로 그대로 <code>PUSH</code>하는 방법을 출력하면 된다.
