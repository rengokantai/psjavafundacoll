#### psjavafundacoll
#####Lists
       get add contains next remove
```
AyyayList    O(1) O(N) O(N) O(1) O(N)
LinkedList   O(N) O(1) O(N) O(1) O(1)
#####Sets
######sortedset and navigableset
tailSet(e)  
headSet(e)  
subSet(e)  
lower(e) higher(e) ceiling(e) pollFirst(e) pollLast(e)
#####Queue and stack
######Queues
add
```
offer(e) return false if queue is full  
add(e) throw exception.  
```
remove
```
if empty, poll() return null
remove() throw exception
```
peek
```
element() throws exception
peek() return null
```
######Priority Queue
```
```
######stack and deque
```
offerFirst(e)
offerLast(e)
addFirst(e)
addLast(e)  //throws exception
getFirst //throws exception
peekFirst
```
######impl
- arraydeque  
ringbuffer based impl  
constant time addition/rem
less memory,faster  
no random access   
- LinkedList  
random access o(n)  
allow null






#####maps
######views over maps
basic api: keySet() values() entrySet()
######sortedmap and navigablemap
SortedMap superceded by NavigableMap.  
firstKey() lastKey() tailMap(k), headMap(k) subMap(k,k)  
firstEntry() lastEntry()  pollfisstEntry...  
lowerEntry(k) lowerKey(k)...

######Java8
replace(key,newval)  replaceAll((id,old)->new Pro(id,old.getName(),old.getW()+10));//8:00
getOrDefault(key,defaultentry) puIfAbsent() compute() computeIfAbsent(10,(id)->new Pro(id,"x",50)) computeIfPresent() merge()
######removeEldestEntry(Map.Entry<k,v> eld)

#####collection operation
######coll algo
```
Collections.rotate(col,1)
Collections.shuffle(col)
Collections.sort(col,field) //or java8, col.sort(field)
```
######collection factories
immutable singleton
```
Set<Integer> set = Collection.singleton(1)
List<Integer> list = Collection.singletonList("one")
Map<Integer,String> map = Collection.singletonMap(1,"one")
```
immutable empty collecton
```
Set<Integer> set = Collection.emptySet()
List<Integer> list = Collection.emptyList()
Map<Integer,String> map = Collection.emptyMap()
```

######utilities
```
Collections.addAll(coll,ele1,ele2,ele3...)
```
