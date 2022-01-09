# `commands-mamba.md`

List environments:

```
mamba info -e
```

Create environment:

```
mamba create -n {environment name} python={python version}
```

Delete environment

```
mamba env remove -n {environment name}
```

Add package to environment

```
mamba activate {environment name}
mamba install {list of packages separated by spaces}
```
