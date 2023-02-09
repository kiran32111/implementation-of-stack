#include <iostream>
using namespace std;

//complete the functions
class Queue{
	int arr[100000];
	int start;
	int end;

	public:
	//constructor is called whenever an object of the class is declared
	Queue(){
		cout<<"constructor is Called\n";
		start=0;
		end=0;

	}

	//push the value at the back
	void push(int val){
		cout<<"pushing the val: "<<val<<" at the back of queue\n";
		
		if(end == size())
            cout << "Queue is Full" << endl;
        else
        {
            arr[end] = val;
            end++;
        }
	}

	int front(){
		cout<<"returning the value at front\n";
		
		if(start == end) {
            return -1;
        }
        else
        {
            return arr[start];
        }
		return 0;
	}

	int pop(){
		cout<<"removing the first element\n";
		
		if(start == end) {
            return -1;
        }
        else
        {	int ans = arr[start];
            arr[start] = -1;
            start++;
            if(start==end){
                start = 0;
                end = 0;
            }
         return ans;
        }
	}

	int size(){
		cout<<"return the size of the queue\n";
		return end;
		return 0;
	}

	bool isEmpty(){
		cout<<"returning if the queue is empty\n";
		
		if(start == end) {
            return true;
        }
        else
        {
            return false;
        }
		return true;
	}
};

int main() {
	Queue q; //constructor is called on this line
	q.push(4);
	cout<<"front: "<<q.front()<<"\n";
	q.pop();
	cout<<"size: "<<q.size()<<"\n";
	cout<<"empty: "<<q.isEmpty()<<"\n";

	q.push(5);
	q.push(3);
	cout<<"front: "<<q.front()<<"\n";
	q.pop();
	cout<<"size: "<<q.size()<<"\n";
	cout<<"empty: "<<q.isEmpty()<<"\n";

	cout<<"front: "<<q.front()<<"\n";
	q.pop();
	cout<<"size: "<<q.size()<<"\n";
	cout<<"empty: "<<q.isEmpty()<<"\n";
	return 0;
}
