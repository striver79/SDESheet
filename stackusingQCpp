class MyStack {
public:
    
    queue<int> que;
    /** Initialize your data structure here. */
    MyStack() {
        
    }
    
    /** Push element x onto stack. */
    void push(int x) {
        que.push(x);
		for(int i=0;i<que.size()-1;++i){
			que.push(que.front());
			que.pop();
		}
    }
    
    /** Removes the element on top of the stack and returns that element. */
    int pop() {
        int x = que.front(); 
        que.pop(); 
        return x; 
    }
    
    /** Get the top element. */
    int top() {
        return que.front();
    }
    
    /** Returns whether the stack is empty. */
    bool empty() {
        return que.size() == 0; 
    }
};
