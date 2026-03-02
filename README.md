# vector_c
A dynamic array implementation for C

### Specialized structures to manage instantiated vector types
typedef struct iter_##_Type {
  vector_##_Type* this;  // pointer to vector
  int type;              // iterator type - enum {_iterator, _reverse_iterator}
  _Type* p;              // pointer to _Val
}iter_##_Type;

### Specialized functions to manage instantiated vector types
iter_##_Type vector_begin(_Type)(vector_##_Type* v);
