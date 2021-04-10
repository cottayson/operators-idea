## Definition of operator
Operator - is a some object that can be represented as arrow between other objects like in Category Theory, but it's hard to say what it is actually without examples.

But we can try:
* operator can be represented as function between objects (denote as OBJ)
* OBJ can be from predefined subset of general types for example:
  + function is OBJ
  + data     is OBJ
  + operator is OBJ
  + some other thing that hard to imagine is OBJ...

## Infinite list of operators
* Forget - used to map state with n properties to state with n - m properties,
  where n, m natural numbers

* Quasi-morphism (or Analogy (or SameAs)) - closely related to isomophism, equivalence classes and invariants.

* AddProbability - used to map 0% and 100% probabity of some event to arbitrary value between 0 and 1.

* AddQuanstumProbability - for example `AddQuanstumProbability(chess) = Quatum chess`

  It can change deterministic algorithms to non-deterministic.
* FunToRel = `One way function to two way or to relation`
  + For example: `f("Simulation of Brownian motion") -> "Brownian bridge"`

* MinimizeComplexity (or Simplify) - obvious, but we can think about minimizing Kolmogorov complexity

* ChangeState - map current state to not equivalent to it, or extend set by one element, that not equivalent to others (find a new element in [Group](https://en.wikipedia.org/wiki/Group_(mathematics)))

## Possible examples of using

### Example 1: Two sides

Given set of objects B = {b_1, b_2, ...} each of which can belong to the "good" and "bad" class(or have some float rating) let's denote this as `isGood(b_i) = {true, false}(or rating: float)`

Suppose the representation of the object is a point on the plane

To avoid a systematic error, we apply mutation operators to an object (or corresponding operations to its representation)

In other words, we change the coordinates (x, y) of a point by a random vector r_j
from the set of random vectors R = {r_1, r_2, ...}, where each is the operator agnalogue over the object x_j

Object visualization:
OBJ_TO_VIS:
b_1 -> Vector2d(x1, y1)
b_2 -> Vector2d(x2, y2)
 ....

Visualization of arrows:
ARROW_TO_VIS:
f_1 -> Vector2d(rx_1, ry_1)
f_2 -> Vector2d(rx_2, ry_2)
...

```hs
OBJ_TO_VIS   :: Object -> Vector2d
ARROW_TO_VIS :: Object -> Vector2d
```

Let it be possible to make estimates
```hs
getRating ::  Object -> Float
```

TO DO continue description...

## Short Two Side idea:
Оценка считается удачной если пользователь смог оценить впринципе(не важно какая оценка положительная или отрицательная важна её фактическая полезность с точки зрения полезной информации)
Первая сторона проблемы при удачной оценке пользователем, что мы может просто её запомнить
Вторая сторона: пользавтель кроме возможности оценки _объекта_, имеет возможность оценки _множество операторов модифицирующих объект_.
