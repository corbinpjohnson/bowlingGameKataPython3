# Bowling Game Kata (Python 3)

[Robert C. Martin's classic Bowling Game Kata](http://www.butunclebob.com/ArticleS.UncleBob.TheBowlingGameKata),
worked in Python 3. The kata builds up a ten-pin bowling scorer test-first, handling the tricky
cases — spares, strikes, and the bonus rolls in the tenth frame.

## What's here

| File | Purpose |
| --- | --- |
| `Game.py` | The scorer: roll pins, then `return_score()` totals the game with spare/strike bonuses |
| `BowlingGameTest.py` | The `unittest` suite that drives the design |

## Run the tests

```bash
python -m unittest BowlingGameTest.py
```

## Usage

```python
from Game import Game

game = Game()
for _ in range(12):   # twelve strikes = a perfect game
    game.roll(10)
print(game.return_score())  # 300
```

## License

[MIT](LICENSE) © Corbin Johnson
