# 문제1 정답
```
#include<stdio.h>
int sum = 0, number[21];
int nachi(int inin) {
	if (inin == 1 || inin == 2) {
		number[inin] = 1;
		return 1;
	}
	else {
		number[inin] = number[inin - 1] + number[inin - 2];
		return number[inin];
	}

}

int main() {
	int what, i, j, much;
	char in;
	scanf("%c", &in);
	scanf("%d", &what);

	for (i = 1; i <= what; i++) {
		much = nachi(i);
		for (j = 0; j < much; j++) {
			printf("%c", in);
		}
		printf("\n");
	}
}
```


# 출제 목적
- 함수를 사용하여 프로그램을 작성할 수 있다.
- 피보나치 수열의 대한 개념을 이해할 수 있다.
- for문을 이용하여 프로그램을 작성할 수 있다.
- 이중 for문을 이용하여 프로그램을 작성할 수 있다.
- 함수에서 ‘return'을 이용하여 값을 반환할 수 있다.
- 배열을 사용할 수 있다.
- 전역변수를 활용하여 프로그램을 작성할 수 있다.
