### (1) Features:
- A sequence of scalar values,
- Constructed using parenthesis and comma, (1,2,3)
- Or using range: (1..100), (a..z)
- Indexed: refer to an element by its position.
- Ordered.
- Elements could be of different types --> complex list
		
### (2) List operator:
- print	
- qw()
    - Quote word: Get a list by extracting words out of a string using space as delimiter.
    - e.g. qw(this is a list)
    - e.g. qw\this is a list\
    - e.g. qw[this is a list]
    - e.g. qw{this is a list}
		
### (3) Flattening list
- `(2,3,4,(5,6))` will be flattened as `(2,3,4,5,6)`
		
### (4) Access list element
- Using 0-based index inside `[]`
- To access one element: `(1,2,3)[0]`
- To access multiple elements: `(4,5,6,3,2)[0,2,3]` --> list slicing
