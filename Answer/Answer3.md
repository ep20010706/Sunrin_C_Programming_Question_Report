# 문제3 정답
```
#include <stdio.h>
int main() {

	int a;
	int b;
	int i, j;
	int cnt = 0;
	int sum = 0;
	int cnt2;
	int done;
	int ho = 0;

	scanf("%d", &a); // a 입력
	scanf("%d", &b); // b 입력

	for (i = 1; i <= a; i++) {
		for (j = 1; j <= i; j++)
			ho++;
		}

	if (ho < b) {
		printf("not found\n");
		return 0;
	}
	
	
	
	for (i = 1; i <= a; i++) {
		for (j = 1; j <= i; j++) {
			sum += j;
			printf("%d ", j);
			cnt++;
			if (cnt == b) {
				cnt2 = j;
				done = sum;
			}
		}

		printf("\n");
	}
	printf("(a%d=%d)", b, cnt2);
	printf("Sigma k=1 to k=%d, ak=%d\n", b, done);

	return 0;
}
```


# 출제 목적
- 이중 if문을 사용할 수 있다.
- 수학식을 코드로 표현할 수 있다.
