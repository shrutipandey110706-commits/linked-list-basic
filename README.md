1)#middle of linked list

class Solution(object):
    def middleNode(self, head):
        slow=head
        fast=head
        while fast and fast.next:
            slow=slow.next
            fast=fast.next,next
        return slow


2)#Reverse linked list
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
