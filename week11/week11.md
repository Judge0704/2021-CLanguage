## 簡化版UVA10082   題目給出英文 讀出各個英文出現幾次
```C  
#include <stdio.h>
char line[2000];
int main()
{
	for(int t=0;gets(line);t++){
		int ans[256]={};
		
		for(int i=0;line[i]!=0;i++){
			char c=line[i];
			ans[c]++;
		}
		if(t>0)printf("\n");
		for(int i=0;i<256;i++){
			if(ans[i]>0)printf("%d %d\n",i,ans[i]);
		}
	}
}
```
