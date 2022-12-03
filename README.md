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



``` python
 # UnoderList
class UnoderList:
      def __init__(self):
            self.head = None

      def isEmpty(self):
            return self.head == None

      def add(self,item):
            temp = Node(item)
            temp.setNext(self.head)
            self.head = temp

      def size(self):
            current = self.head
            count = 0
            while current != None:
                  count = count + 1
                  current = current.getNext()
            return count

      # searches for the item in the list. It needs the item and returns a boolean value.
      def search(self,item):
            pass
      
      # Menghapus nilai dari suatu Unorderlist
      def remove(self,item):
            pass
      
      # adds a new item to the end of the list making it the last item in the col- lection. 
      # It needs the item and returns nothing. Assume the item is not already in the list.
      def append(self, item):
            pass
      
      # returns the position of item in the list. It needs the item and returns the index. Assume the item is in the list
      def index(self, item):
            pass
      
      # adds a new item to the list at position pos. It needs the item and returns nothing. 
      # Assume the item is not already in the list and there are enough existing items to have position pos.
      def insert(self, pos, item):
            pass
      
      # removes and returns the last item in the list. 
      # It needs nothing and returns an item. Assume the list has at least one item
      def pop(self):
            pass 
      
      # removes and returns the item at position pos. 
      # It needs the position and returns the item. Assume the item is in the list
      def pop(self, pos):
            pass
      
      # mencetak nilai di dalam unorderlist 
      def cetak(self):
            pass
           
 ```


``` python 

# Testing/Pengecekan
MyUnorderList = UnoderList()
print(MyUnorderList.isEmpty())
MyUnorderList.add(10)
MyUnorderList.add(100)
MyUnorderList.add(1) # 1, 100, 10
MyUnorderList.cetak()
MyUnorderList.remove(100)
MyUnorderList.cetak() # 1, 10

print(MyUnorderList.size())
print(MyUnorderList.search(1))
MyUnorderList.cetak()


```
