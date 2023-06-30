# Pescapp

## Especies

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

## Especie

### **Get** single especie

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

### **Create** especie

`[POST]: .../app/src/api/especies/`

> REQUEST:

 ```json
{ 	
	"nombre":"Pulpo común"
	"nombreCientifico":"Octopus Vulgaris",
	"fao":"OCC",
	"imagen":"pulpo_comun.jpg"
} 
```
> RESPONSE:

```json
{
	"completed": true,
	"especie": { 	
			"id":"1",
			"nombre":"Pulpo común",
			"nombreCientifico":"Octopus Vulgaris",
			"fao":"OCC",
			"imagen":"pulpo_comun.jpg"
		   }
}
```

> ERROR:

```json
{
	"completed": false,
	"error": "No se ha insertado correctamente en la BD."
}
```

### **Update** especie

`[POST]: .../app/src/api/especies/`

> REQUEST:

```json
{ 	
	"id":"1",
	"nombre":"Pulpo común",
	"nombreCientifico":"Octopus Vulgaris",
	"fao":"OCC",
	"imagen":"pulpo_comun.jpg"
} 
```

> RESPONSE:

```json
{
	"completed": true,
	"especie": { 	
			"id":"1",
			"nombre":"Pulpo común",
			"nombreCientifico":"Octopus Vulgaris",
			"fao":"OCC",
			"imagen":"pulpo_comun.jpg"
		   }
}
```

> ERROR:

```json
{
	"completed": false,
	"error": "No se ha actualizado correctamente en la BD."
}
```

------------

## Zonas de capturas

`[GET]: .../app/src/api/zonas_capturas/`

```json
[{
	"id":"1",
	"nombre":"Zona 27.IX.a - Atlántico, nordeste"
 } , ...]
```

## Zona de captura

### **Get** single zona de captura


`[GET]: .../app/src/api/zonas_capturas/?id=1`

```json
 {
	"id":"1",
	"nombre":"Zona 27.IX.a - Atlántico, nordeste"
 } 
```

### **Create** zona de captura

`[POST]: .../app/src/api/zonas_capturas/`

> REQUEST:

```json
 {
	"nombre":"Zona 27.IX.a - Atlántico, nordeste"
 } 
```

> RESPONSE:

```json
{
	"completed": true,
	"zonaCaptura": { 	
			"id":"1",
			"nombre":"Zona 27.IX.a - Atlántico, nordeste"
		   }
}
```

> ERROR:

```json
{
	"completed": false,
	"error": "No se ha insertado correctamente en la BD."
}
```

### **Update** zona de captura

`[POST]: .../app/src/api/zonas_capturas/`

> REQUEST:

```json
 {
	"id":"1",
	"nombre":"Zona 27.IX.a - Atlántico, nordeste"
 } 
```

> RESPONSE:

```json
{
	"completed": true,
	"zonaCaptura": { 	
			"id":"1",
			"nombre":"Zona 27.IX.a - Atlántico, nordeste"
		   }
}
```

> ERROR:

```json
{
	"completed": false,
	"error": "No se ha actualizado correctamente en la BD."
}
```


`[GET]: .../app/src/api/especies/`

```json
{
	"id":"570",
	"proveedor":{
		"id":"12",
		"nombre":"La Cabriola",
		"tipo":"1",
		"razonSocial":"-",
		"nif":"-",
		"direccion":"-",
		"poblacion":"Conil ",
		"cp":"11140",
		"pais":"España"
	},
	"fecha":"2023-06-30",
	"estado":"0",
	"lineasArticulos":[],
	"lineasArticulosMateriasPrimas":[{},{},{}],
	"lineasArticulosEspeciales":[{}],
	"lineasDescuentos":[],
	"agrupado":0,
	"subtotal":380,
	"descuentos":null,
	"baseImponible":380,
	"impuestos":null,
	"importeTotal":380,
	"cantidadTotal":45
}
```
