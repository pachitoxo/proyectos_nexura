---
{"dg-publish":true,"fecha producción":"6/08/2021","Url:":"https://www.pereira.gov.co/gfiles/20/tramitevirtual/","permalink":"/alcaldia-de-pereira/tramite-licencia-de-cremacion-e-inhumacion-de-cadaveres/","dgPassFrontmatter":true}
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



# Historia de Usuario #LicenciaImhumación


## Modelo Entidad Relación: 

``` mermaid 
classDiagram
    UsuariosPermitdos --|> tnGiflesFunerarias
  
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