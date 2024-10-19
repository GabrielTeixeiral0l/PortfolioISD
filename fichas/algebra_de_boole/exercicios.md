# Exercícios Álgebra de Boole &nbsp; [![Ir para README](https://img.shields.io/badge/Indice-Verde?style=for-the-badge)](../../README.md#indice)

```
A + A . B  = A

A + A x B = A.(1+B)
		  = A . (1)
		  = A
```

```
A.(A+B) = A

A . (A + B) = A . A + A . B
            = A + A . B
            = A (1 + B)
            = A (1)
            = A
```

```
A + A' . B = A + B

A + A' . B = (A + A' . B)''
           = (A' . (A + B'))''
           = (A'. A + A' . B')'
           = (0 + A' . B')'
           = (A' . B')'
           = A + B
```

```
(A + B) . (A + C) = A + B . C

(A + B) . (A + C) = A . A + A . C + B . A + B . C
                  = A + A . C + B . A + B . C
                  = A . C + A . B + B . C
                  = A + A . (C + B) + B . C
                  = A . (1 + (C + B)) + B . C
                  = A . 1 + B . C
                  = A + B . C
```
