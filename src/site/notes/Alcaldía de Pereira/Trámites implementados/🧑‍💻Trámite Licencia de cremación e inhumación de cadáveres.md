---
{"dg-publish":true,"permalink":"/alcaldia-de-pereira/tramites-implementados/tramite-licencia-de-cremacion-e-inhumacion-de-cadaveres/"}
---


>Autorización para enterrar o depositar cadáveres, restos óseos y partes humanas en los cementerios.

# Ficha técnica del trámite:

- [ ] ¿Requiere pago?  
- [x] Frecuencia anual de 1560 solicitudes
- [ ] ¿Requiere integración?
- [x] ¿Requiere expedir certificado?
- [x] Personalizaciones
- [x] Activado en producción desde 6/08/2021
- [x] Url de producción: https://www.pereira.gov.co/gfiles/20/tramitevirtual/




```mermaid
pie title transacciones anuales
    "Transacciones total anual" : 45326
    "Transacciones concepto sanitario" : 1560
```

# Flujo de proceso

![Pasted image 20230919094711.png](/img/user/Pasted%20image%2020230919094711.png)



# Historia de Usuario #LicenciaImhumación


## Diagrama de clase: 

``` mermaid 
classDiagram
    UsuariosPermitidos --|> tnGiflesFunerarias
  
    class tnGiflesFunerarias{
      +id (pk) int(11)
      +nombre varchar(225)
      +email varchar(225)  
    }
   
```

## Lógica funcional:


``` mermaid 
sequenceDiagram

    Ciudadano->>+Sistema: Iniciar sesión
    Ciudadano->>+Sistema: “licencia para inhumación y cremación de cadáveres”
    Sistema-->>-Ciudadano: No se muestra el formulario para radicar la solicitud.
    Sistema-->>-Ciudadano: “Usted no cuenta con acceso permitido para realizar este trámite”

```