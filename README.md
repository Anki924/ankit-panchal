#include<iostream>
using namespace std;

class employee{
    public:
    int sal=0;
    employee(){}
    employee(){
        int id=0;
        cout<<"Enter your id\n";
        cin>>id;
    }
};

class salary : public employee{
    public:
        salary(){}
    void get(){
        cout<<"Enter your salary\n";
        cin>>sal;
        // }
    // void inc(int sal){
        if(sal>10000){
            cout<<"now your salary is "<<sal+2000<<endl;
        }
        else{
            cout<<"you are ok"<<endl;
        // }
    }  
};

class display:public employee,public salary{
    void dis(){
        employee e;
        salary pr;
        pr.get();
        
    }
};
int main(){
    
    display ankit,devesh;

    return 0;
}
