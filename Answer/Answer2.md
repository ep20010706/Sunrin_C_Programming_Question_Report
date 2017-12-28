# 문제2 정답
```
#include<stdio.h>
int main() {
	int basicmoney, basicdis, moredis, moremoney, godis, i, j, arrive, total;
	scanf("%d %d", &basicmoney, &basicdis);
	scanf("%d %d", &moremoney, &moredis);
	scanf("%d", &godis);
	arrive = godis - basicdis;
	total = basicmoney;

	while (arrive > 0) {
		total += moremoney;
		arrive = arrive - moredis;
	}
	printf("busfee = %d\n", total);
}

```


# 출제 목적
- while문을 이용하여 프로그램을 작성할 수 있다.
- for문을 쓰기 않고 간결하게 프로그램을 작성할 수 있다.

