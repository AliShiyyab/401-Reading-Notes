# HashMap

> *Have a many number of algorithem*

> *Google used HashTable*

> *Used hashtable to save the thing which i used daily like wikipedia website used daily*

> *Example*

* Have an empty array of size 8
* i need to put the 10 in the empty array
* where i need to put it ?
    * the first step is used `10 % 8 = 2` -> put `10` in the index number **2**
    * the number is 20 -> 20 % 8 = 4 put `20` in the index number **4**
    * the number is 18 -> 18 % 8 = 2 put `18` in the index number thats mean i need to delete the 10 from the hash and swapped to put `18` 

## Function hash are have:

* **init**
* **insert**
* **find**
* **remove**

## Init

>create table of M lists

## Insert(K)

index = h(K)

insert into table[index]

## Find(K)

index = h(K)

walk down list at table[index], looking for a match return what was found (or error)

## Remove(K)

index = h(K)

walk down list at table[index], lookiing for a match remove what was found (or error)

