# ����3 ����
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

	scanf("%d", &a); // a �Է�
	scanf("%d", &b); // b �Է�

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


# ���� ����
- ���� if���� ����� �� �ִ�.
- ���н��� �ڵ�� ǥ���� �� �ִ�.
