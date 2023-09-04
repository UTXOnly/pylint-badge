# pybadge ![pylint Score](pylint.svg)

pylint badges for everyone!

## Howto

Run the `pylintbadge.py` script located in the `pylintbadege` directory, pass the files or directories you want lited as arguments.

For example:

```
python3 pylintbadge.py ./*.py ./docker_stuff/python_stuff/*.py
```
You'll then see the Pylint output displayed to the console. YOu can check your score here.

```
************* Module nost_query
nost_query.py:72:35: E1101: Module 'secp256k1' has no 'Error' member (no-member)
nost_query.py:86:12: W0622: Redefining built-in 'id' (redefined-builtin)
nost_query.py:80:15: E1101: Module 'websockets' has no 'connect' member (no-member)
nost_query.py:83:12: W0612: Unused variable 'i' (unused-variable)
nost_query.py:98:15: E1101: Module 'websockets' has no 'connect' member (no-member)
nost_query.py:115:12: W0612: Unused variable 'i' (unused-variable)
nost_query.py:7:0: C0411: standard import "import time" should be placed before "import secp256k1" (wrong-import-order)
------------------------------------------------------------------
Your code has been rated at 8.79/10 (previous run: 9.21/10, -0.42)
```
If the script runs without any errors, you will also see confirmation that the file was created in the directory.
```
pylint.svg written
```

## Adding the badge to your profile

If your badge is produced in the same directory as your `Readme.md` you can simply add the following to your `Readme.md` :
```
![Pylint_score](./pylint.svg)
```

## Color intervals

0.00 < ![pylint Score](https://mperlet.github.io/pybadge/badges/1.50.svg) < 3.00 < ![pylint Score](https://mperlet.github.io/pybadge/badges/5.51.svg) < 7.00 ![pylint Score](https://mperlet.github.io/pybadge/badges/9.73.svg) < 10.00

## Limitations

* negative scores are not supported

## Idea
Inspired by mperlet's [pybadge](https://github.com/mperlet/pybadge), which was in turn inspired by [this blogpost](http://www.desmondrivet.com/blog/technical/pylint-badges.html.)
