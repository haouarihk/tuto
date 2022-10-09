# types of diagrams
Each type has it's own focus,

## Dynamic:
Describes the operations, actions, and changes that occur in a system over time

## Static:
Describes the state of a system from a variety of perspectives

## functional:
showcases the functions of each part of the system

## Class:
Object oriented, showcases the properties and association between them in terms of just the ownership of data.
same as static but with associations

| name           |     |
| -------------- | --- |
| properties     |     |
||     |
| -------------- |     |
| operations     |     |
| -------------- |     |
|  responsability                |     |

- **+**: Public
- **-**: Private
- #: Preview

### operations
```rule
Visibility OperationName(paramName:Type):returnType
```



## Aggregation and Composition:

- $\diamond$ Aggregation(formation, grouping): use it when the connected item isn't part of parent, or when the parent gets deleted the connected item wont also get deleted.

- $\bullet$ composition(constitution, made-up):  use it when the connected  item is part of the parent, or when the parent gets deleted the connected item will also get deleted.


## Generalisation:
when you go from child to parent in the graph