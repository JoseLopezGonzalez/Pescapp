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

`[PUT] o [PATCH]: .../app/src/api/especies/`

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

`[PUT]: .../app/src/api/zonas_capturas/`
· No tiene posibilidad de PATCH (ya que solo tiene una propiedad o atributo)

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

------------

## Barcos

`[GET]: .../app/src/api/proveedores/barcos`

```json
[{
        "id": "1",
        "nombre": "Bellita Cale",
        "tipo": "1",
        "razonSocial": "-",
        "nif": "-",
        "direccion": "-",
        "poblacion": "Isla Cristina",
        "cp": "21410",
        "pais": "España",
        "matricula": "3SE-1-11-04",
        "cfr": "ESP000026188",
        "contrato": "0"
 }, ...]
```

## Barco

### **Get** single barco


`[GET]: .../app/src/api/proveedores/barcos/?id=1`

```json
 {
        "id": "1",
        "nombre": "Bellita Cale",
        "tipo": "1",
        "razonSocial": "-",
        "nif": "-",
        "direccion": "-",
        "poblacion": "Isla Cristina",
        "cp": "21410",
        "pais": "España",
        "matricula": "3SE-1-11-04",
        "cfr": "ESP000026188",
        "contrato": "0"
 }
```

### **Create** barco

`[POST]: .../app/src/api/proveedores/barcos/`

> REQUEST:

```json
 {
        "nombre": "Bellita Cale",
        "tipo": "1",
        "razonSocial": "-",
        "nif": "-",
        "direccion": "-",
        "poblacion": "Isla Cristina",
        "cp": "21410",
        "pais": "España",
        "matricula": "3SE-1-11-04",
        "cfr": "ESP000026188",
        "contrato": "0"
 }
```

> RESPONSE:

```json
{
	"completed": true,
	"barco": {
		        "id": "1",
		        "nombre": "Bellita Cale",
		        "tipo": "1",
		        "razonSocial": "-",
		        "nif": "-",
		        "direccion": "-",
		        "poblacion": "Isla Cristina",
		        "cp": "21410",
		        "pais": "España",
		        "matricula": "3SE-1-11-04",
		        "cfr": "ESP000026188",
		        "contrato": "0"
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

### **Update** barco

`[PUT] o [PATCH]: .../app/src/api/proveedores/barcos/`

> REQUEST:

```json
 {
        "id": "1",
        "nombre": "Bellita Cale",
        "tipo": "1",
        "razonSocial": "-",
        "nif": "-",
        "direccion": "-",
        "poblacion": "Isla Cristina",
        "cp": "21410",
        "pais": "España",
        "matricula": "3SE-1-11-04",
        "cfr": "ESP000026188",
        "contrato": "0"
 }
```

> RESPONSE:

```json
{
	"completed": true,
	"barco": {
		        "id": "1",
		        "nombre": "Bellita Cale",
		        "tipo": "1",
		        "razonSocial": "-",
		        "nif": "-",
		        "direccion": "-",
		        "poblacion": "Isla Cristina",
		        "cp": "21410",
		        "pais": "España",
		        "matricula": "3SE-1-11-04",
		        "cfr": "ESP000026188",
		        "contrato": "0"
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



