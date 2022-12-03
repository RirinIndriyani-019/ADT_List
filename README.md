# ADT_List
``` python

class Node:
      def __init__(self,data:None):
            self.data = data
            self.next = None
            
      def getData(self):
            return self.data
      
      def getNext(self):
            return self.next
      
      def setData(self,newdata):
            self.data = newdata
            
      def setNext(self,newnext):
            self.next = newnext

# Testing/Pengecekan
n1 = Node(10)
n2 = Node('a')
n3 = Node(12)

n1.setNext(n3)
n3.setNext(n2)

c = n1
while c :
    print(c.data)
    c = c.next
```
