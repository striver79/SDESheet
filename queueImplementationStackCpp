class MyQueue {
public:
    stack<int> input, output;
    /** Initialize your data structure here. */
    MyQueue() {
        
    }
    
    /** Push element x to the back of queue. */
    void push(int x) {
        input.push(x);
    }
    
    /** Removes the element from in front of queue and returns that element. */
    int pop() {
        // shift input to output 
        if (output.empty())
            while (input.size())
                output.push(input.top()), input.pop();

        int x = output.top();
        output.pop(); 
        return x; 
    }
    
    /** Get the front element. */
    int peek() {
        // shift input to output 
        if (output.empty())
            while (input.size())
                output.push(input.top()), input.pop();
        return output.top(); 
    }
    
    /** Returns whether the queue is empty. */
    bool empty() {
        return input.empty() && output.empty();
    }

};
