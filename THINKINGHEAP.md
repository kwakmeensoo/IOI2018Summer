# THINKING HEAP
### 문제 설명
수업 시간에 O(lg N) 만에 삽입과 삭제가 가능한 자료구조인 Heap을 배운 민수는 Heap을 이용해 여러가지 숫자를 <code>PUSH</code>하고 <code>POP</code>한 결과, Heap에 <code>PUSH</code>한 순서에 따라 Heap의 내부에 저장되는 순서가 다르다는 걸 깨달았다.
Heap에 1 ~ N까지의 숫자를 <code>PUSH</code>할 때, i번째 인덱스에 K가 위치하는 <code>PUSH</code> 방법을 출력하시오.
### 입력
첫째 줄에, i(1 ≤ i ≤ N)와 K(1 ≤ K ≤ N)가 주어진다. Heap의 인덱스 번호는 1부터 시작한다고 가정한다.
### 출력
가능한 <code>PUSH</code> 방법 중, **아무거나 한 가지**를 출력하시오. 그러한 방법이 없다면 -1을 출력하시오.
