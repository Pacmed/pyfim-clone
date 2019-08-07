# pyfim clone

Clone of pyfim making it installable as a dependency. Copied from http://www.borgelt.net/pyfim.html

# installation
`pip install git+https://github.com/Pacmed/pyfim-clone`

Now we can import pyfim (from python):

`from fim import fpgrowth`

# include in your project

If you would like to include pyfim as a dependency for your project, simply add this to your `setup.py` file:
```python    
setup(
    ...
    install_requires=[
        'fim @ git+https://github.com/Pacmed/pyfim-clone',              
    ],
    ...
)
```

Alternatively, you can add it via these lines:
```python    
setup(
    ...
    install_requires=[
        'fim',
    ],
    dependency_links=[
        'https://github.com/Pacmed/pyfim-clone/tarball/master#egg=fim-6.28'
    ],
    ...
)
```
