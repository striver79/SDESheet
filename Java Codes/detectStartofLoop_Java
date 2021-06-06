/**
 * Definition for singly-linked list.
 * class ListNode {
 *     int val;
 *     ListNode next;
 *     ListNode(int x) {
 *         val = x;
 *         next = null;
 *     }
 * }
 */
public class Solution {
    public ListNode detectCycle(ListNode head) {
        if (head == null || head.next == null)
            return null;
    
        ListNode slow  = head;
        ListNode fast  = head;
        ListNode entry = head;

        while (fast.next!=null && fast.next.next!=null) {
            slow = slow.next;
            fast = fast.next.next;
            if (slow == fast) {                      // there is a cycle
                while(slow != entry) {               // found the entry location
                    slow  = slow.next;
                    entry = entry.next;
                }
                return entry;
            }
        }
        return null;       
    }
}
