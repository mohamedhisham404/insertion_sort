#include<iostream>
#include<string>

using namespace std;

void showarr(int arr[],int size)
{
    for(int i=0;i<size;i++)
    {
        cout<<arr[i]<<"\t";
    }
}

void InsertionSortASC(int arr[],int size)
{
    for(int step=1; step < size ;step++)
    {
        int key = arr[step];
        int j = step -1;

        while(key < arr[j] && j>=0)
        {
            arr[j+1] = arr[j];
            --j;
        }
        arr[j + 1] = key;   
    }
}

void InsertionSortDES(int arr[],int size)
{
    for(int step=1; step < size ;step++)
    {
        int key = arr[step];
        int j = step -1;

        while(key > arr[j] && j>=0)
        {
            arr[j+1] = arr[j];
            --j;
        }
        arr[j + 1] = key;   
    }
}

int main()
{
    int data[6];
    int size = sizeof(data) / sizeof(data[0]);
    int option;
    
    do
    {
        cout<<"*************************INSERTION SORT*************************"<<endl;
        cout<<"ENTER 0 TO EXIT"<<endl;
        cout<<"INTER THE NUMBERS YOU WANT TO SORT(6 numbers only)"<<endl;
        for(int i=0;i<6;i++)
        {
            cin>>data[i];
        }
        cout<<"DO YOU WANT IT IN ASC OR DES ORDER?"<<endl;
        cout<<"1. ASC"<<endl;
        cout<<"2. DES"<<endl;
        cin>>option;

        switch (option)
        {
        case 1:
            cout<<"THIS IS YOUR NUMBERS IN ASC ORDER :"<<endl;
            InsertionSortASC(data,size);
            showarr(data,size);
            break;
        
        case 2:
            cout<<"THIS IS YOUR NUMBERS IN DES ORDER :"<<endl;
            InsertionSortDES(data,size);
            showarr(data,size);
            break;
        default:
            break;
        }
    } while (option != 0);
    
    
    
    
    // int data[]={66,21,54,62,98,69,62};
    // int size = sizeof(data) / sizeof(data[0]);
    // InsertionSort(data,size);
    // cout<<"SORTED ARRAY IS: \n"<<endl;
    // showarr(data,size);

    return 0;
}
