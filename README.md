The Bowling Game Kata
=====================
#### Based on a [slideshow][1] by Sebastian Bergmann

---


Game Rules
----------

Bowling consists of ten frames.  Two balls are rolled in the first nine frames, three can be rolled on the tenth.  The score is based on the total number of pins knocked down each frame, including bonuses for spares and strikes.  A spare occus when a player knocks down all ten pins in one roll. The number of pins knocked down on the next roll are added to the spare as a bonus.  A strike occurs when a player knocks down all ten pins in one roll. This adds the value of the next two frames to the strike frame as a bonus.  If a player rolls a spare or strike on the tenth frame, they are allowed to roll extra balls to complete the frame for a total of three.

#### Score poorly mocked up below

```
 ------  ----  ------  ----  ------  ----  ------  ----  ------ -------
| 2 |3 | 4 |2 | 3 |5 | 7 |/ | 6 |/ | 5 |3 |   |X | 8 |1 | 6 |/ | 3|/|X |
|    5 |   11 |   17 |   33 |   48 |   56 |   75 |   84 |   97 |   127 |
 ------  ----  ------  ----  ------  ----  ------  ----  ------ -------
```


Planning
--------

### `BowlingGame`

#### `roll($pins)`
- Called each time the ball is rolled
 - `$pins` is the number of pins knocked down

#### `score()`
- Called at the end of the game and returns the score


[1]: http://www.slideshare.net/dpc/quality-assurance-in-php-projects-sebastian-bergmann