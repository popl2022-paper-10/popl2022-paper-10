Trustworthy Program Verification via Proof Generation
----------------------------

## Requirements

The following are required:
  - PyPy 3.7+
  - Python 3.7+

Then run the following to install dependencies for Python and PyPy
```
python3 -m pip install -r requirements.txt
pypy3 -m pip install -r requirements.txt
```

## Statistics
  - See `examples/popl22/stats/*.mm.time` for proof generation time
  - See `examples/popl22/stats/*.mm.verify.time` for checking time using mmverify.py
  - See `examples/popl22/stats/*.mm.compressed-verify.time` for checking time using mmverify.py and decompression

## Reproducing the stats

```
$ cd examples/popl22
$ make all               # to generate proofs
$ make compress          # to compress proofs
$ make verify            # to generate stats/*.mm.verify.time
$ make compressed-verify # to generate stats/*.mm.compressed-verify.time
```
