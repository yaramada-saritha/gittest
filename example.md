# A Heading

Some Description which explains the topic as an overview.

Bullet points here:
* One
* Two

## Overview done

* Refresh the screen

* an image to insert below ![image](demo1.gif)

> An excerpt included in a line here

if no changes needed this will not be an excerpt.

```plantuml
@startuml component
actor client
node app
database db

db -> app
app -> client
@enduml
```
Here is another one

```graphviz
digraph finite_state_machine {
    rankdir=LR;
    size="8,5"

    node [shape = doublecircle]; S;
    node [shape = point ]; qi

    node [shape = circle];
    qi -> S;
    S  -> q1 [ label = "a" ];
    S  -> S  [ label = "a" ];
    q1 -> S  [ label = "a" ];
    q1 -> q2 [ label = "ddb" ];
    q2 -> q1 [ label = "b" ];
    q2 -> q2 [ label = "b" ];
}
```


```graphviz
digraph G {
    graph [rankdir = LR, splines=ortho];

    node[shape=record];
    Bar[label="Bar", height=2];
    Foo[label="Foo", height=4];

    Bew[label="Bew", height=2];

    Bar -> Foo [label="Bar2Foo"];
    Bar -> Foo [label="Bar2Foo"];
    Bar -> Foo [label="Bar2Foo"];

    Bew -> Foo [label="Bew2Foo"];
    Foo -> Bew [label="Foo2Bew"];
    Foo -> Bew [label="Foo2Bew"];
    

}
```

```graphviz
digraph X {
    Gate[label="Gate", height=2];
    graph [rankdir = LR, splines=ortho];
    Foo -> Gate [label="Foo2Gate"];
    Foo -> Gate [label="Foo2Gate"];
}

```