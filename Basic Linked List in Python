class LinkedList:
    def __init__(self):
        self.head= None #set the head iniitial value to be null
    
    def insertnode(self,data):
        llnode = node(data)
        if not self.head:
            self.head = llnode
        else:
            self.tail.next=llnode
        self.tail=llnode
    
    def printlist(self):
        ptr=self.head
        while(ptr!=None):
            print(ptr.data,end="__--->")
            ptr=ptr.next
        print("▯")
        
    def get(self,n):
        ptr=self.head
        i=0
        while(ptr!=None and i<n):
#             print(ptr.data)
            ptr=ptr.next
            i+=1
#         print(i)
        if(ptr==None):
            print("Index out of range of Elements in LinkedList")
        else:
            print(ptr.data)
    
    def search(self,ele):
        ptr=self.head
        i=0
        while(ptr!=None):
            if ptr.data==ele:
                print("Element is present in the list")
                return i
            i+=1
            ptr=ptr.next
        print("Element not present")
        return -1
    def insertat(self,n,data):
        nd = node(data)
        if(n==0):
            temp=self.head
            self.head=nd
            nd.next=temp
        else:
            ptr=self.head
            i=0
            while(ptr!=None and i<n-1):
                ptr=ptr.next
                i+=1
            if(ptr==None):
                assert False,"Index not in the list"
            else:
                nd.next=ptr.next
                ptr.next=nd
#                 print(nd.next.data)

    def delnode(self,n):
        if(n==0):
            self.head=self.head.next
        else:
            ptr=self.head
#             print(ptr.data)
            i=0
            while(ptr!=None and i<n-1):
#                 print(i)
                ptr=ptr.next
                i+=1
            if(ptr==None):
                assert False,"Index not in the list"
            else:
                ptr.next=ptr.next.next
    def rev(self):
        ptr=self.head
        prev=None
        while(ptr is not None):
            new=ptr.next
            ptr.next=prev
            prev=ptr
            ptr=new
        self.head=prev
        
class node:
    def __init__(self,data):
        self.data=data
        self.next=None
    
# For Example Consider this Linked List named List    
linked = LinkedList()
linked.insertnode(13)
linked.insertnode(16)
linked.insertnode(18)
linked.insertnode(133)
linked.insertnode(17)   
