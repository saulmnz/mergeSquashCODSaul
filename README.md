
# 1ER commit main/master
```bash

"LE AÑADIMOS CONTENIDO AL README"

git add README.md
git commit -m "Primer Commit"

```

# 2DO commit main/master

```bash
"LE AÑADIMOS CONTENIDO AL README"

git add README.md
git commit -m "Segundo Commit"
```
# Crea la rama de colaborador

```bash

git checkout -b colaborador

# commit a
"LE AÑADIMOS CONTENIDO AL README"
git add README.md
git commit -m "A"

```bash
# commit B
"LE AÑADIMOS CONTENIDO AL README"
git add README.md
git commit -m "B"

```

# commit C
```bash
"LE AÑADIMOS CONTENIDO AL README"
git add README.md
git commit -m "C"
git push
```


## PARTE DE LIDER

# Creamos la rama en la que vamos a trabajar
```bash
git checkout -b lider
```

# HACER UN COMMIT
```bash
git add .\README.md
git commit -m "L1"
```

# HACER OTRO COMMIT
````bash
git add .\README.md
git commit -m "L2"
````

# ULTIMO COMMIT
```bash
git add .\README.md
git commit -m "C"
```


# MERGE DE LA RAMA LIDER
```bash
# vamos a la rama main
git checkout main

# cargamos los cambios del colaborador
git pull

# hacemos el merge squash con la rama lider
git merge --squash líder

# solo faltará corregir los conflictos y ya
git commit -m "squash listo líder"
git push
```
