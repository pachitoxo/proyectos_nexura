---
{"dg-publish":true,"fecha producción":"6/08/2021","permalink":"/alcaldia-de-pereira/tramite-beneficio-predial/","dgPassFrontmatter":true}
---

>Descuento para el pago predial del siguiente año.

# Ficha técnica del trámite:

- [ ] ¿Requiere pago?  
- [x] Frecuencia anual de 1560 solicitudes
- [ ] ¿Requiere integración?
- [x] ¿Requiere expedir certificado?
- [x] Personalizaciones
- [x] Activado en producción desde 6/08/2021
- [x] Url de producción: https://www.pereira.gov.co/gfiles/47/tramitevirtual/


## Flujo de proceso:

![Pasted image 20230911155820.png](/img/user/Pasted%20image%2020230911155820.png)

# Historia de Usuario #BeneficioPredial


## Modelo Entidad Relación: 

```mermaid 
classDiagram
    UsuariosPermitdos --|> tnGiflesFunerarias
  
    class tnGiflesFunerarias{
      +id (pk) int(11)
      +nombre varchar(225)
      +email varchar(225)  
    }
```




```mermaid 
	graph LR;
		A -> B
```



Personalización:

``` javascript

# Leer la primera línea (encabezados)
        encabezados = next(lector_csv)
        
        # Verificar la estructura de los encabezados
        if len(encabezados) != 3 or encabezados != ['columna1', 'columna2', 'columna3']:
            raise ValueError("La estructura del archivo CSV es incorrecta.")
        
        # Continuar con la carga y procesamiento del archivo
       # Agregar la lógica para procesar cada fila del archivo
        
        for fila in lector_csv:
            # Procesar la fila del archivo
            # Imprimir los valores de cada columna
            
            columna1 = fila[0]
            columna2 = fila[1]
            columna3 = fila[2]
            
      print(f"Valor columna1: {columna1}, Valor columna2: {columna2}, Valor columna3: {columna3}")

``` 