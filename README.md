# Pescapp

# Especies

`[GET]: .../app/src/api/especies/`

```json
[ { 	
	"id":"1",
	"nombre":"Pulpo común",
	"nombreCientifico":"Octopus Vulgaris",
	"fao":"OCC",
	"imagen":"pulpo_comun.jpg" 
 } , ...]
```

### Especie

`[GET]: .../app/src/api/especies/?id=1`

```json
 { 	
	"id":"1",
	"nombre":"Pulpo común",
	"nombreCientifico":"Octopus Vulgaris",
	"fao":"OCC",
	"imagen":"pulpo_comun.jpg" 
 } 
```

------------

# Zonas de capturas

`[GET]: .../app/src/api/zonas_capturas/`

```json
[{
	"id":"1",
	"nombre":"Zona 27.IX.a - Atlántico, nordeste"
 } , ...]
```

### Zona de captura

`[GET]: .../app/src/api/zonas_capturas/?id=1`

```json
 {
	"id":"1",
	"nombre":"Zona 27.IX.a - Atlántico, nordeste"
 } 
```
