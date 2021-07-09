## Tests
If you add new steps, you need to create a small data for integration tests. There is a test example in `celescope/tests/test_multi.py`. To run this example:


1. Get test data
```
# If you have access to Singleron Nanjing HPC
copy -r /SGRNJ03/randd/user/zhouyiqi/multi_tests/test_folder {test_dir}
# Or clone from repo
git clone https://github.com/singleron-RD/celescope_tests.git
```

2. Run `pytest`
```
Install pytest
>>> pip install pytest
Run all
>>> python -m pytest -s ./tests/test_multi.py --test_dir {test_dir}
Run some tests
>>> python -m pytest -s ./tests/test_multi.py --test_dir {test_dir} --assays rna,tag
```

Then you need to create your own test based on this example.