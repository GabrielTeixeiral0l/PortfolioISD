# Ficha de trabalho - simplificações &nbsp; [![Ir para README](https://img.shields.io/badge/Indice-Verde?style=for-the-badge)](../../README.md#indice)

1. Simplifique: 
```
A . B + A . B' + A' . B' = A (B + B') + A' . B'
				 = A  + A' . B'
				 = A + B'
```

``` 
A . B . C .  A + A . B' . C' + A' . B + A' . B' + A . B . A'  
	= (A . B . C .  A) +( A . B' . C') + (A' . B) + (A' . B') + (A . B . A')
    = (A . B . C) +  (A . B' . C') + (A' . B) + (A' . B') + (0 . B)
    = (A . B . C) + (A' . B) + (A . B' . C') + (A' . B')
    = A (B . C + B' . C') + A' (B + B')
	= A (B . C + B' . C') + A' (1)
	= A (B . C + B' . C') + A' 
```

``` 
A . C' + A . B . A' + A . B . C . A + B . B . C' + B . A'
	= (A . C') + (A . B . A')+ (A . B . C . A) + (B . B . C') + (B . A')
	= (A . C') + (0 . B) + (A . B . C) + (B . C') + (B . A')
	= (A . C') + (A . B . C) + (B . C') + (B . A')
	= A (C' + (B . C)) + (B . C') + (B . A')
	= A (B + C') + (B . C') + (B . A')
	= AB + AC' + BC' + BA'
	= B (A + A') + AC' + BC'
	= B (1) + AC' + BC'
	= B + AC' + BC'
	= B + BC' + AC'
	= B + AC'
```

```  
 (A . B . C) + (C . A . B) + (A . B) + A
	= (A . B . C) + (A . B) + A
	= (A . B . C) + A
``` 	

``` 
(B . C) + (A . D) + (A . B . C . D) + (C . D . A) + A'
	= (B . C) + (B . C . A . D) + (A . D) + (C . D . A) + A'
	= (B . C) + (A . D) + (C . D . A) + A'
	= BC + AD + A'
```

``` 
(A' . B . C) + (A . B' . C') + (A . B' . C) + (A . B . C') + (A . B . C)
	 = BC (A + A') + (A . B' . C') + (A . B' . C) + (A . B . C')
	 = BC + AB' (C' + C) + (A . B . C')
	 = (BC) + (AB') + (A . B . C')
``` 

``` 
((A . (A . B)')' . (B . (A . B)')')'
	= (A . (A . B)' + B . (A . B)')
	= (A . (A' + B') + B . (A' + B'))
```

``` 
(A'+B')' + A + A . (B . C . D)' =
	= (A' . B') + A + A . B' . C' . D'
	= (A' . B') + A + (A . B' . C' . D')
	= (A' . B') + A 
```

``` 
(A . B + C) . (A + B) . C
	= ABA + ABB + CA + CB . C
	= AB + AB + CA + CB . C
	= AB + CA + CBC
``` 

2. Demonstre que  (A + B) . (A' + C) = (A + B) . (A' + C) . (B + C)
   
``` 
(A + B) . (A' + C) . (B + C) =
	= (A + B)  (A' . B + A' . C + C . B + C . C)
	= (A + B)  (A' . B + A' . C + C . B + C)
	= BA' + BA'C + CB + AC + BC
	= BA' + BA'C + BC + AC
	= BA' +BC(A + 1) + AC
	= BA' + BC + AC
``` 	
	NOTA:
```
(A + B) . A' . B = A . A'B  + B . A'B = 0 B + BA' = BA'
(A + B) . A' . C = A. A'C + B . A'C = 0 B + BA'C = BA'C
(A + B) . CB = ACB + BCB = ACB + BC = CB (A + 1) = CB
(A + B) . C = AC + BC
```
	
``` 
	(A + B) . (A' + C) =
		= AA' + AC + BA' + BC
		= AC + BA' + BC
		= BA' + BC + AC
``` 

	
3. Demonstre que (A + B) . (A' + C) = (A + B) . (B + C) . (A' + C .(B + C))

``` 
	(A + B) . (A' + C) =
		= AA' + AC + BA' + BC
		= 0 + AC + BA' + BC
		= **AC + BA' + BC**
		
	(A + B) . (B + C) . (A' + C . (B + C))
		= (AB + AC + BB + BC) . (A' + C . (B + C))
		= (AB + AC + B + BC) . (A' + C)
		= ABA' + ACA' + BA' + BCA' + ABC + ACC + BC + BCC 
		= 0 + 0 + BA' + BCA' + ABC + AC + BC + BC 
		= BA' + BCA' + ABC + AC + BC 
		= BA' + AC + BC
		= **AC + BA' + BC**
	
``` 
