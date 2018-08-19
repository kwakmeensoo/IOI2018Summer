# 퇴교(EXPLUSION)
https://algospot.com/judge/problem/read/WITHDRAWAL

실수 범위의 Parametric Search를 할 때 조건문이 아닌 100번의 루프를 돌려 찾는 것이 안전하다.

    for(int loop = 0; loop < 100; ++loop) {
        ...
    }
