# sphinx_demo
Demo of sphinx document generation

# Clone the repo and open index.html in any browser

# The documetation is generate using sphinx with these commands:
```
git clone https://github.com/pandas-dev/pandas.git
# Use pandas directory only in the repo
make html
sphinx-apidoc -o ./rst/ ./src/pandas/
cd rst
mv modules.rst index.rst
cp ../conf.py .
mkdir _static
sphinx-build -b html ./rst/ ./html
```
