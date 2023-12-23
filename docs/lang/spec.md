# Built in types
type number
type string

# Built in functions

# Build in effects
effect eval = string -> nothing



# Table of needs
|                | Abstract Definition | Concrete Definition | Concrete Implementation | Pure Lambda | Pure Data |
| :------------- | :-----------------: | :-----------------: | :---------------------: | :---------: | :-------: |
| function       |          X          |                     |                         |      X      |           |
| behavior       |                     |          X          |                         |      X      |           |
| trait          |                     |          X          |                         |             |           |
| implementation |                     |                     |            X            |             |           |
| type           |          X          |                     |                         |             |     X     |
| data           |                     |          X          |                         |             |     X     |
| effect         |          X          |                     |                         |             |           |

abstract function af = { }
abstract effect ae = { }
abstract behavior ab = { }
abstract trait at = { }
abstract data ad = { }

concrete function f impl af,ab,at = { }
concrete effect e impl af,ae,ab,at = { }
concrete behavior b impl ab = { }
concrete trait t impl at = { }
concrete data d impl ad = { }