1)# remove the given value form the linked list

class Solution(object):
    def removeElements(self, head, val):
        """
        :type head: Optional[ListNode]
        :type val: int
        :rtype: Optional[ListNode]
        """
        dummy=ListNode(0)#dummy 
        dummy.next=head 
        current = dummy
        while current.next:
            if current.next.val==val:
                current.next=current.next.next #removes the value
            else:
                current = current.next #moves to next to check 
        return dummy.next    
2)#middle of linked list

class Solution(object):
    def middleNode(self, head):
        slow=head
        fast=head
        while fast and fast.next:
            slow=slow.next
            fast=fast.next,next
        return slow


3)#Reverse linked list
class solution(object):
    def ReverseList(self,head):
        temp=head
        prev=None
        while temp is not None:
            front=temp.next  #stores the next node
            temp.next=prev   #reerse link
            prev=temp        #moves prev forward
            temp=front       #moves temp forward
        return prev    
