# Install

`conda create -n poke_replay python=3.11 --yes`

`conda activate poke_play`

`pip install -r requirements.txt`

# Add ROM

The Pokémon Red Rom should be located at the path `./PokemonRed.gb`. Otherwise specify the path using `--rom my_rom.gb`.

# Record playthrough

`python play.py --name my_replay.pkl`

Controls:

```
action_mapping = {
    pygame.K_UP: 3,
    pygame.K_DOWN: 0,
    pygame.K_LEFT: 1,
    pygame.K_RIGHT: 2,
    pygame.K_a: 4, # A
    pygame.K_s: 5, # B
    pygame.K_RETURN: 6,
}
```

Note that the key A is used for `A` and the key S is used for `B`. Change this to your likings. I did this because of the different local keyboard layouts.

When done recording, press Q or just quit.

# Replay

`python replay.py --name my_replay.pkl`
