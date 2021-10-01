class Solution {
public:
    ListNode* mergeTwoLists(ListNode* l1, ListNode* l2) {
        // iterative 
        ListNode* res = new ListNode(); 
        ListNode *temp = res; 
        
        while(l1 != NULL && l2!=NULL) {
            if(l1->val < l2->val) {
                res->next = l1; 
                res = res -> next; 
                l1 = l1->next; 
            }
            else {
                res->next = l2; 
                res = res->next; 
                l2 = l2->next; 
            }
        }
        while(l1 != NULL) {
            res->next = l1; 
            res = res -> next; 
            l1 = l1->next; 
        }
        while(l2 != NULL) {
            res->next = l2; 
            res = res -> next; 
            l2 = l2->next; 
        }
        
        return temp->next;
    }
};
