#include <iostream>

using namespace std;
int linearSearch(int array[],int size, int searchValue)
{
    for(int i = 0;i < size; i++){
        if (searchValue == array[i]){
            return i;
        }
    }
    return -1;
}

int main(){
    
    int a[][] = {1, 3, 6 ,10 , 13, 90, 12,89, 53, 70, 23, 3},
                {7,0,0,0};
    
    int uservalue;
    
    cout<<"enter an int: "<<endl;
    cin>> uservalue;
    
    int b =linearSearch(a, 6, uservalue);
    
    if(result >= 0){
         cout<<"the number " << a[result] " was found at the element with index"<< result<<endl;
    }else{
        cout<<"the number "<< uservalue <<"was not found. "<< endl;
    }
}
