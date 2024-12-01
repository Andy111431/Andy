泡沫排序法
#include <iostream>
using namespace std;

void bubble_sort(int a[], int n){
	for(int i=0; i<n-1; i++)
		for(int j=0; j<n-1-i; j++)
			if(a[j] > a[j+1])
				swap(a[j], a[j+1]);
}

int main(){
    int a[10] = {6,9,4,8,7,1,3,5,2,0};
    bubble_sort(a, 10);
    for(int i=0; i<10; i++){
        cout << a[i] << ' ';
    }
}
