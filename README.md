# Link to the list :https://www.geeksforgeeks.org/top-20-linked-list-interview-question/

#Find the middle of a given linked list
class Solution
{
    int getMiddle(Node head)
    {
         // Your code here.
        Node temp = head;
        int count =0 ;
        while(temp!=null){
            count += 1;
            temp = temp.next;}
        temp = head;
        int i=0;
        while(i<count/2){
            temp = temp.next;
            i++;
        }
         
    return temp.data;
    }
}
