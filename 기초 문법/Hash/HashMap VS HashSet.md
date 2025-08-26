## HashMap과 HashSet차이
<br>

### 1. 인터페이스
HashMap은 Map 인터페이스의 구현체로 **<key, value>** 쌍으로 저장한다.
HashSet은 Set 인터페이스의 구현체로 내부적으로 HashMap을 사용하며, value대신 **key**로 저장한다.

### 2. 구성
HashMap은 <key,value>로 구성되며 key는 중복이 안되지만 **value는 중복**이 될 수 있다.
따라서 map.put("apple", 3), map.put("banana", 3) 이런식으로 저장해도 다르게 인식된다.

HashSet은 HashMap의 key로 저장하기에 **중복이 안된다**.
따라서 set.add("apple")과 같이 이런식으로 저장하며 중복된 키 값을 넣을 수 없다.

### 3. 속도
HashMap과 HashSet모두 해시테이블 기반이기에 검색, 삽입, 삭제가 모두 O(1)속도로, 큰 차이는 없으며 빠르다
