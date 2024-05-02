//3.배열,구조체,포인터 오류를 수정하라.
#include <stdio.h>
#include <stdlib.h>

int main() {
    double* p1;
    p1 = (double*)malloc(sizeof(double)); // double 형식의 메모리 블록 할당
    *p1 = 23.92; // 할당된 메모리 블록에 값을 저장

    // 메모리 블록을 더 이상 사용하지 않을 때는 반드시 해제해야 함
    free(p1);

    return 0;
}
