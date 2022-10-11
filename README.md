# c++_love
C++ 打印爱心

在控制台输出爱心



## 源代码

```c++
// 打印爱心
#include <stdio.h>
#include <stdlib.h>
#include <Windows.h>

int main() {
	float x, y, a;
	for(y=1.5; y>-1.5; y-=0.1){
		for (x = -1.5; x < 1.5; x += 0.05) {
			a = x * x + y * y - 1;
			putchar(a * a * a - x * x * y * y * y <= 0.0 ? '*' : ' ');
		}
		system("color 0c");
		putchar('\n');
	}
	return 0;
}

```


## 效果如图：


![image](https://user-images.githubusercontent.com/32007383/195121273-982681bb-70bf-4397-a62d-7fdf9cfe119e.png)


