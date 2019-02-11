# Crowd Remover
Remove annoying crowds from a non-stable movie, taken with a hand camera.


## Source Codes
- detect_objejct_from_movie.py: Extract the background from a stable movie.

```bash
    $ python detect_objejct_from_movie.py [input].mp4 [output]
```

- anti_shake_byECC.py: Stabilize an image with warpMatrix to maximize ECC between two frames.

```bash
    $ python anti_shake_byECC.py [input].mp4 [output]
```

- hconcat.py: concatenate two movies horizontally.

```bash
    $ python hconcat.py [left].mp4 [right].mp4 [output]
```

- utils.py: Utilities for visualize the foreground.

## Result

- Top-left: The original movie
- Bottom-left: Removing crowds without stabilization
- Top-right: The stabilized movie
- Bottom-right: Removing crowds with stabilization

![result](./akamon.gif "result")
