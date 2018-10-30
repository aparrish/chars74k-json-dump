# Converting English Hand-Drawn Chars74k Data to JSON

By [Allison Parrish](http://www.decontextualize.com/)

This is just a quick notebook to convert the stroke trajectories of the
hand-drawn English letters in the
[Chars74k](http://www.ee.surrey.ac.uk/CVSSP/demos/chars74k/) dataset to JSON.
See [the notebook](chars74k-json-dump.ipynb) for more details.

You can download the JSON-converted files directly. The JSON object
maps each letter in the dataset (0-9, a-z, A-Z) to a list of letterforms (55 for
each letter), which in turn are lists of [x, y] coordinates for
each point in the stroke.

* [Regular](https://github.com/aparrish/chars74k-json-dump/raw/master/char74k.json)
* [Normalized](https://github.com/aparrish/chars74k-json-dump/raw/master/char74k-normalized.json)
  (translated so that each letterform is centered on the center of the strokes'
  bounding box)

Here's [an example of the data in
use](https://editor.p5js.org/allison.parrish/sketches/r1mIgSInQ).

## License

The code and text herein is licensed as
[CC0](https://creativecommons.org/share-your-work/public-domain/cc0/). The data
in the JSON files is governed by the [reuse rules accompanying the original
paper](http://www.ee.surrey.ac.uk/CVSSP/demos/chars74k/).

