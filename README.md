# vector_c
A dynamic array implementation for C

### Specialized structures to manage instantiated vector types
typedef struct iter_##_Type {<br />
&nbsp;&nbsp;&nbsp;&nbsp;vector_##_Type* this;&nbsp;// pointer to vector<br />
&nbsp;&nbsp;&nbsp;&nbsp;int type;&nbsp;// iterator type - enum {_iterator, _reverse_iterator}<br />
&nbsp;&nbsp;&nbsp;&nbsp;_Type* p; &nbsp;// pointer to _Val<br />
}iter_##_Type;<br />

### Specialized functions to manage instantiated vector types
iter_##_Type vector_begin(_Type)(vector_##_Type* v);
