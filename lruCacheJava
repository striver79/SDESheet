class LRUCache {  
  Node head = new Node(0, 0), tail = new Node(0, 0);
  Map<Integer, Node> map = new HashMap();
  int capacity;
  
  public LRUCache(int _capacity) {
    capacity = _capacity;
    head.next = tail;
    tail.prev = head;
  }

  public int get(int key) {
    if(map.containsKey(key)) {
      Node node = map.get(key);
      remove(node);
      insert(node);
      return node.value;
    } else {
      return -1;
    }
  }

  public void put(int key, int value) {
    if(map.containsKey(key)) {
      remove(map.get(key));
    }
    if(map.size() == capacity) {
      remove(tail.prev);
    }
    insert(new Node(key, value));
  }
  
  private void remove(Node node) {
    map.remove(node.key);
    node.prev.next = node.next;
    node.next.prev = node.prev;
  }
  
  private void insert(Node node){
    map.put(node.key, node);
    node.next = head.next;
    node.next.prev = node;
    head.next = node;
    node.prev = head;
  }
  
  class Node{
    Node prev, next;
    int key, value;
    Node(int _key, int _value) {
      key = _key;
      value = _value;
    }
  }
}

/**
 * Your LRUCache object will be instantiated and called as such:
 * LRUCache obj = new LRUCache(capacity);
 * int param_1 = obj.get(key);
 * obj.put(key,value);
 */
