# vector_c
A dynamic array implementation for C

### Specialized structures to manage instantiated vector types
typedef struct iter_##_Type {<br />
  vector_##_Type* this;  // pointer to vector<br />
  int type;              // iterator type - enum {_iterator, _reverse_iterator}<br />
  _Type* p;              // pointer to _Val<br />
}iter_##_Type;<br />

### Specialized functions to manage instantiated vector types
iter_##_Type vector_begin(_Type)(vector_##_Type* v);
