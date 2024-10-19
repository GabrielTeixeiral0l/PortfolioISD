# Ficha de trabalho - simplificações &nbsp; [![Ir para README](https://img.shields.io/badge/Indice-Verde?style=for-the-badge)](../../README.md#indice)

1. Simplifique:

```
A . (A . B + C) = A . ((A . B) + C)
		= A . (A . B) + A . C
		= (A . A . B) + (A . C)
		= (A . B) + (A . C)
        =  A . (B + C)
```

```
A . B + A . B' + A' . B' = (A . B + A . B' + A' . B')''
                = (A' + B' . A' + B' . A + B)'
                = (A' + B' . A + B .(A' + B))'
                = (1 . (A' + B))'
                =  A + B'
```

```
A . B . C .  A + A . B' . C' + A' . B + A' . B' + A . B . A'
	= (A . B . C .  A) +( A . B' . C') + (A' . B) + (A' . B') + (A . B . A')
    = (A . B . C) +  (A . B' . C') + (A' . B) + (A' . B') + (0 . B)
    = (A . B . C) + (A' . B) + (A . B' . C') + (A' . B')
    = (B . ((A . C) + A')) + (A . B' . C') + (A' . B')
	= (B . (A' + C)) + (A . B' . C') + (A' . B')
	= (B . (A' + C)) + ((( A ⋅ C') + A' ) ⋅ B')
    = (B . (A' + C)) + ((A' . C') ⋅ B')
    = (B . A') + (B . C) + (B' . A') + (B' . C')
    = (B . A') + (B' .  A') + (B . C) + (B' . C')
    = (A' (B + B')) + (B . C) + (B' . C')
    = (A' (1)) + (B . C) + (B' . C')
    =  A' + (B . C) + (B' . C')
```

```
A . C' + A . B . A' + A . B . C . A + B . B . C' + B . A'
	= (A . C') + (A . B . A')+ (A . B . C . A) + (B . B . C') + (B . A')
	= (A . C') + (0 . B) + (A . B . C) + (B . C') + (B . A')
	= (A . C') + (A . B . C) + (B . C') + (B . A')
	= (A . C') + (B . ((A . 1 . C) + (1 . C') + (1 . A')))
	= (A . C') + (B . ((A . C) + (C') + (A')))
	= (A . C') + (B . A . C) + (B . C') + (B . A')
	= (A . C') + (B . A') + (B . A . C)
	= (A . ((B . C) + (C'))) + (B . A')
	= (A . (C' + B)) + (B . A')
	= (A . C') + (A . B) + (B . A')
	= (B ((A) + (A'))) + (A . C')
	= (B (1)) + (A . C')
	=  B + (A . C')
```

2. Demonstre que

3. Demonstre que
