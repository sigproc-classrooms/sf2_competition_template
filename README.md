# SF2 Competition entry

This is a template repository for your competition entry.
Your repository must provide the three functions within the `competition` module:

* `header_bits`
* `encode`
* `decode`

To help you get started, we've preloaded this template with an encoder that uses `jpegenc` and
`jpegdec`, along with the `opthuff` argument to build the header.

Note that this respository does not include a copy of `cued_sf2_lab`, but will find the version that you alraedy have installed.
As such, you **should not modify your `cued_sf2_lab`**, as the demonstrators will not have this version installed.
If you need to make changes to the function in that package, you should copy the files into this repository.

For development, you can import these functions in Jupyter with
```python
from competition import header_bits, encode, decode
```

In the competition, we will run this using
```bash
python -m cued_sf2_lab.competition_runner competition thecompetition_image
```
Where `competition` is the name of this directory.
This will write out your decoded images as `png` files into the `outputs` directory, along with a `pickle` file containing your encoded data.
If you right click out `outputs/summary.md` in VSCode and click "Open preview", you can see the competition results.
