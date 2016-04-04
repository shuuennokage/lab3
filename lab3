#include <iostream>
#include <fstream>
#include <vector>
using namespace std;

int main() {
	ifstream fin;
	fin.open("file.in");
	int size=0, value=0, i, count=0, temp, sumMax=0;
	vector<int> Suuryou;
	Suuryou.clear();
	
	while (fin>>value){
		size = value;
		Suuryou.resize(size);
			for (i=0; i<size; i++){
			while (fin>>value){
				Suuryou[i] = value;
				break;
			}
		}
		break;
	}
	for (i=1; i<size;){
		goOn:
		if (i-count>0){
			if (Suuryou[i-count]>Suuryou[i-1-count]){
				temp = Suuryou[i-count];
				Suuryou[i-count] = Suuryou[i-(count+1)];
				Suuryou[i-(count+1)] = temp;
				count++;
				goto goOn;
			}else {
				count = 0;
				i++;
			}
		}else {
			count = 0;
			i++;
		}	
	}
	
	for (i=0; i<5; i++){
		sumMax += Suuryou[i];
	}
	cout << sumMax <<endl;
	fin.close();
	return 0;
}
