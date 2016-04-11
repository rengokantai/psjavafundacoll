#### psjavafundacoll
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
