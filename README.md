# wcag-mathcat-for-python
Repository containing MathCAT implementation in Rust. It includes instructions how to use this code as Python package. MathCAT is used in math formulas conversions to natural language.

In order to build Python package from Rust code follow below step:

1. Create virtual environment.
2. Install requirements.txt. It contains package ```maturin```, which is used for Rust compilation.
3. Go to MathCAT directory.
4. Run ```maturin build``` or ```maturin develop``` in order to prepare ```.whl``` file.

Path to generated ```.whl``` file should be found in the logs of previous maturin command.

**Warning!** In order to perform step 4, you need to have Rust compiler installed.

5. Now you can install package from ```.whl``` file in any project you need. 

Note that interface that is available from Python package is defined in ```<MathCAT_directory_path>/src/lib.rs```
