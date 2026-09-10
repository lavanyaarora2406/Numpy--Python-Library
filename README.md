import pypandoc

readme = """# NumPy

A compact set of NumPy notebooks covering fundamentals, advanced operations, and practical tricks.

## Topics

### Fundamentals
- NumPy basics, arrays & matrices
- Array attributes & operations
- Scalar & vector operations
- Dot product
- Mathematical & statistical functions
- Slicing & iteration
- Reshaping
- Stacking & splitting

### Advanced NumPy
- NumPy arrays vs Python lists
- Advanced, fancy & boolean indexing
- Broadcasting
- Mathematical operations
- Sigmoid & Mean Squared Error
- Missing values
- Plotting with NumPy

### NumPy Tricks
- Sort, append & concatenate
- Percentile & flip
- Set operations
- Useful NumPy functions & shortcuts

## Notebooks

- `numpy_fundamentals.ipynb`
- `numpy_advanced.ipynb`
- `numpy_tricks.ipynb`
"""

path = "/mnt/data/README.md"
pypandoc.convert_text(readme, "md", format="md", outputfile=path, extra_args=["--standalone"])
print(path)
