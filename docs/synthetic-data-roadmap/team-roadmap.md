![Alt text](https://g.gravizo.com/source/team_roadmap?https://raw.githubusercontent.com/mcleo-d/datahub/add-team-roadmap/docs/synthetic-data-roadmap/team-roadmap.md)

<details> 
<summary></summary>
team_roadmap
  digraph G {
    size ="4,4";
    main [shape=box];
    main -> parse [weight=8];
    parse -> execute;
    main -> init [style=dotted];
    main -> cleanup;
    execute -> { make_string; printf};
    init -> make_string;
    edge [color=red];
    main -> printf [style=bold,label="100 times"];
    make_string [label="make a string"];
    node [shape=box,style=filled,color=".7 .3 1.0"];
    execute -> compare;
  }
custom_mark10
</details>