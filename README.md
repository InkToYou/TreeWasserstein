# TreeWasserstein
A python module for fast calculation of the wasserstein distance on tree metrics implemented by C++.

# Requirements
`Python 3.7.3` + `pipenv` + `Clang 11.0.0`

# Usage

## Setup
```
pipenv install Pipfile
```

## Build
```
pipenv run make build
```

## Test
``` 
pipenv run make test
```

## Example
``` 
import tw
first_prob = [0, 0, 1]
second_prob = [1 / 3, 1 / 3, 1 / 3]
edges = [(0, 1, 1), (0, 2, 1)]
tw.distance(first_prob, second_prob, edges) # 1.0
 ```

## Performance
See [here](examples/example.ipynb)


# Reference
- https://arxiv.org/abs/1005.1699
- https://arxiv.org/abs/1902.00342
- https://pot.readthedocs.io/en/stable/#
- https://networkx.github.io/
