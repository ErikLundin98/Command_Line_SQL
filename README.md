# Command line SQL tool

I was inspired by [q](http://harelba.github.io/q/), which is a tool to execute sql queries on files from the command line, and decided to try to create a (much simpler, and therefore slower and less functional) version of it.

# Install

Run:
```python
pip install -r requirements.txt
```

# Usage

## With python

Call the script ```fql.py``` followed by the query. Example:

```
> "SELECT * FROM test_data/test.csv JOIN test_data/test_copy.csv"
```

# Run from anywhere

## Windows

Add the path of the repository to your PATH variable. Then, you can run ```fql.bat``` from anywhere in the following way:

```
./fql <QUERY>
```

## Linux

Run the following command to make the file executable:

```
chmod +x fql
```

Add it to path, using e.g.
```
set PATH=%PATH%;%CD%
```
Then, you can run the script using

```
./fql <QUERY>
```
# Supported file formats

extensions = ["csv", "tsv", "dat", "log"]
