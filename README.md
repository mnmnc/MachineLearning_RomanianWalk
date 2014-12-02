MachineLearning_RomanianWalk
============================

Travel from romaninan cities to Bucharest based on direct distances. Greedy Algorithm.

## INPUT
```python
dist = {
        'Bucharest':            0,
        'Giurgiu':              77,
        'Urziceni':             80,
        'Pitesti':              98,
        'Craiova':              160,
        'Fagaras':              178,
        'Rimnicu Vilcea':       193,
        'Mehadia':              241,
        'Dobreta':              242,
        'Lugoj':                244,
        'Sibiu':                253,
        'Timisoara':            329,
        'Arad':                 366,
        'Zerind':               374,
        'Oradea':               380
}

neighbours = {
        'Giurgiu':              ['Bucharest'],
        'Fagaras':              ['Bucharest', 'Sibiu'],
        'Lugoj':                ['Timisoara', 'Mehadia'],
        'Mehadia':              ['Dobreta', 'Lugoj'],
        'Oradea':               ['Zerind', 'Sibiu'],
        'Timisoara':            ['Arad', 'Lugoj'],
        'Zerind':               ['Arad', 'Oradea'],
        'Arad':                 ['Zerind', 'Timisoara', 'Sibiu'],
        'Craiova':              ['Dobreta', 'Rimnicu Vilcea', 'Pitesti'],
        'Pitesti':              ['Bucharest', 'Rimnicu Vilcea', 'Craiova' ],
        'Dobreta':              ['Mehadia', 'Craiova' ],
        'Rimnicu Vilcea':       ['Pitesti', 'Craiova',  'Sibiu'],
        'Bucharest':            ['Urziceni', 'Giurgiu', 'Pitesti', 'Fagaras'],
        'Sibiu':                ['Oradea', 'Fagaras', 'Arad', 'Rimnicu Vilcea']
}

```

## OUTPUT
```python
  Starting travel from Arad
           Sibiu
           Fagaras
           Bucharest
  Destination reached!
  Travel ended in Bucharest
```

