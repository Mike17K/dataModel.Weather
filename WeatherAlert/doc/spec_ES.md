<!-- 10-Header -->  
[![Smart Data Models](https://smartdatamodels.org/wp-content/uploads/2022/01/SmartDataModels_logo.png "Logo")](https://smartdatamodels.org)  
Entidad: WeatherAlert  
=====================<!-- /10-Header -->  
<!-- 15-License -->  
[Licencia abierta](https://github.com/smart-data-models//dataModel.Weather/blob/master/WeatherAlert/LICENSE.md)  
[documento generado automáticamente](https://docs.google.com/presentation/d/e/2PACX-1vTs-Ng5dIAwkg91oTTUdt8ua7woBXhPnwavZ0FxgR8BsAI_Ek3C5q97Nd94HS8KhP-r_quD4H0fgyt3/pub?start=false&loop=false&delayms=3000#slide=id.gb715ace035_0_60)  
<!-- /15-License -->  
<!-- 20-Description -->  
Descripción global: **Una alerta meteorológica generada por un usuario o dispositivo en un lugar determinado**.  
versión: 0.3.1  
<!-- /20-Description -->  
<!-- 30-PropertiesList -->  

## Lista de propiedades  

<sup><sub>[*] Si no hay un tipo en un atributo es porque puede tener varios tipos o diferentes formatos/patrones</sub></sup>.  
- `address[object]`: La dirección postal  . Model: [https://schema.org/address](https://schema.org/address)	- `addressCountry[string]`: El país. Por ejemplo, España  . Model: [https://schema.org/addressCountry](https://schema.org/addressCountry)  
	- `addressLocality[string]`: La localidad en la que se encuentra la dirección postal, y que está en la región  . Model: [https://schema.org/addressLocality](https://schema.org/addressLocality)  
	- `addressRegion[string]`: La región en la que se encuentra la localidad, y que está en el país  . Model: [https://schema.org/addressRegion](https://schema.org/addressRegion)  
	- `district[string]`: Un distrito es un tipo de división administrativa que, en algunos países, gestiona el gobierno local    
	- `postOfficeBoxNumber[string]`: El número del apartado de correos para las direcciones de apartados postales. Por ejemplo, 03578  . Model: [https://schema.org/postOfficeBoxNumber](https://schema.org/postOfficeBoxNumber)  
	- `postalCode[string]`: El código postal. Por ejemplo, 24004  . Model: [https://schema.org/https://schema.org/postalCode](https://schema.org/https://schema.org/postalCode)  
	- `streetAddress[string]`: La dirección  . Model: [https://schema.org/streetAddress](https://schema.org/streetAddress)  
	- `streetNr[string]`: Número que identifica una propiedad específica en una vía pública    
- `alertSource[*]`: Fuente de la alerta  . Model: [http://schema.org/URL](http://schema.org/URL)- `alternateName[string]`: Un nombre alternativo para este artículo  - `areaServed[string]`: La zona geográfica en la que se presta un servicio o se ofrece un artículo  . Model: [https://schema.org/Text](https://schema.org/Text)- `category[string]`: Categoría de la entidad  - `data[object]`: Carga útil que contiene los datos recuperados  - `dataProvider[string]`: Una secuencia de caracteres que identifica al proveedor de la entidad de datos armonizada  - `dateCreated[date-time]`: Fecha de creación de la entidad. Normalmente será asignada por la plataforma de almacenamiento  - `dateIssued[date-time]`: La fecha y la hora de emisión en formato ISO8601 UTC  . Model: [https://schema.org/DateTime](https://schema.org/DateTime)- `dateModified[date-time]`: Marca de tiempo de la última modificación de la entidad. Suele ser asignada por la plataforma de almacenamiento  - `description[string]`: Descripción de este artículo  - `id[*]`: Identificador único de la entidad  - `location[*]`: Referencia Geojson al elemento. Puede ser Point, LineString, Polygon, MultiPoint, MultiLineString o MultiPolygon.  - `name[string]`: El nombre de este artículo  - `owner[array]`: Una lista que contiene una secuencia de caracteres codificada en JSON que hace referencia a los identificadores únicos de los propietarios.  - `seeAlso[*]`: lista de uri que apuntan a recursos adicionales sobre el artículo  - `severity[string]`: Gravedad de la alarma  - `source[string]`: Secuencia de caracteres que indica la fuente original de los datos de la entidad en forma de URL. Se recomienda que sea el nombre de dominio completo del proveedor de origen o la URL del objeto de origen.  - `subCategory[string]`: Categorías meteorológicas. Enum:' avalanchas, evento costero, ola de frío, inundación, niebla, incendio forestal, ola de calor, alta temperatura, huracán, hielo, baja temperatura, precipitación, lluvia_inundación, nieve, nieve_hielo, tormentas eléctricas, tornado, ciclón tropical, tsunami, viento'.  - `type[string]`: Tipo de entidad NGSI. Tiene que ser WeatherAlert  - `validFrom[date-time]`: Inicio del período de validez de esta previsión en formato ISO8601  . Model: [https://schema.org/DateTime](https://schema.org/DateTime)- `validTo[date-time]`: Fin del período de validez de esta previsión en formato ISO8601  . Model: [https://schema.org/DateTime](https://schema.org/DateTime)<!-- /30-PropertiesList -->  
<!-- 35-RequiredProperties -->  
Propiedades requeridas  
- `alertSource`  - `category`  - `dateIssued`  - `id`  - `subCategory`  - `type`  <!-- /35-RequiredProperties -->  
<!-- 40-RequiredProperties -->  
Esta carpeta contiene todos los artefactos de software para ofrecer datos de alerta meteorológica en NGSI v2. La fuente de estos datos es el [Servicio Europeo de Alarma Meteorológica] global (http://meteoalarm.eu).  
<!-- /40-RequiredProperties -->  
<!-- 50-DataModelHeader -->  
## Descripción de las propiedades del modelo de datos  
Ordenados alfabéticamente (pulse para más detalles)  
<!-- /50-DataModelHeader -->  
<!-- 60-ModelYaml -->  
<details><summary><strong>full yaml details</strong></summary>    
```yaml  
WeatherAlert:    
  description: A weather alert generated by a user or device in a given location    
  properties:    
    address:    
      description: The mailing address    
      properties:    
        addressCountry:    
          description: 'The country. For example, Spain'    
          type: string    
          x-ngsi:    
            model: https://schema.org/addressCountry    
            type: Property    
        addressLocality:    
          description: 'The locality in which the street address is, and which is in the region'    
          type: string    
          x-ngsi:    
            model: https://schema.org/addressLocality    
            type: Property    
        addressRegion:    
          description: 'The region in which the locality is, and which is in the country'    
          type: string    
          x-ngsi:    
            model: https://schema.org/addressRegion    
            type: Property    
        district:    
          description: 'A district is a type of administrative division that, in some countries, is managed by the local government'    
          type: string    
          x-ngsi:    
            type: Property    
        postOfficeBoxNumber:    
          description: 'The post office box number for PO box addresses. For example, 03578'    
          type: string    
          x-ngsi:    
            model: https://schema.org/postOfficeBoxNumber    
            type: Property    
        postalCode:    
          description: 'The postal code. For example, 24004'    
          type: string    
          x-ngsi:    
            model: https://schema.org/https://schema.org/postalCode    
            type: Property    
        streetAddress:    
          description: The street address    
          type: string    
          x-ngsi:    
            model: https://schema.org/streetAddress    
            type: Property    
        streetNr:    
          description: Number identifying a specific property on a public street    
          type: string    
          x-ngsi:    
            type: Property    
      type: object    
      x-ngsi:    
        model: https://schema.org/address    
        type: Property    
    alertSource:    
      anyOf:    
        - description: Identifier format of any NGSI entity    
          maxLength: 256    
          minLength: 1    
          pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
          type: string    
          x-ngsi:    
            type: Property    
        - description: Identifier format of any NGSI entity    
          format: uri    
          type: string    
          x-ngsi:    
            type: Property    
      description: Source of the alert    
      x-ngsi:    
        model: http://schema.org/URL    
        type: Relationship    
    alternateName:    
      description: An alternative name for this item    
      type: string    
      x-ngsi:    
        type: Property    
    areaServed:    
      description: The geographic area where a service or offered item is provided    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    category:    
      description: 'Category of the Alert. Enum:''traffic, naturalDisaster, weather, environment, health, security, agriculture'''    
      enum:    
        - traffic    
        - naturalDisaster    
        - weather    
        - environment    
        - health    
        - security    
        - agriculture    
      type: string    
      x-ngsi:    
        type: Property    
    data:    
      description: Payload containing the data retrieved    
      type: object    
      x-ngsi:    
        type: Property    
    dataProvider:    
      description: A sequence of characters identifying the provider of the harmonised data entity    
      type: string    
      x-ngsi:    
        type: Property    
    dateCreated:    
      description: Entity creation timestamp. This will usually be allocated by the storage platform    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    dateIssued:    
      description: The date and time the item was issued in ISO8601 UTC format    
      format: date-time    
      type: string    
      x-ngsi:    
        model: https://schema.org/DateTime    
        type: Property    
    dateModified:    
      description: Timestamp of the last modification of the entity. This will usually be allocated by the storage platform    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    description:    
      description: A description of this item    
      type: string    
      x-ngsi:    
        type: Property    
    id:    
      anyOf:    
        - description: Identifier format of any NGSI entity    
          maxLength: 256    
          minLength: 1    
          pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
          type: string    
          x-ngsi:    
            type: Property    
        - description: Identifier format of any NGSI entity    
          format: uri    
          type: string    
          x-ngsi:    
            type: Property    
      description: Unique identifier of the entity    
      x-ngsi:    
        type: Property    
    location:    
      description: 'Geojson reference to the item. It can be Point, LineString, Polygon, MultiPoint, MultiLineString or MultiPolygon'    
      oneOf:    
        - description: Geojson reference to the item. Point    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                type: number    
              minItems: 2    
              type: array    
            type:    
              enum:    
                - Point    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON Point    
          type: object    
          x-ngsi:    
            type: GeoProperty    
        - description: Geojson reference to the item. LineString    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  type: number    
                minItems: 2    
                type: array    
              minItems: 2    
              type: array    
            type:    
              enum:    
                - LineString    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON LineString    
          type: object    
          x-ngsi:    
            type: GeoProperty    
        - description: Geojson reference to the item. Polygon    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  items:    
                    type: number    
                  minItems: 2    
                  type: array    
                minItems: 4    
                type: array    
              type: array    
            type:    
              enum:    
                - Polygon    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON Polygon    
          type: object    
          x-ngsi:    
            type: GeoProperty    
        - description: Geojson reference to the item. MultiPoint    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  type: number    
                minItems: 2    
                type: array    
              type: array    
            type:    
              enum:    
                - MultiPoint    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON MultiPoint    
          type: object    
          x-ngsi:    
            type: GeoProperty    
        - description: Geojson reference to the item. MultiLineString    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  items:    
                    type: number    
                  minItems: 2    
                  type: array    
                minItems: 2    
                type: array    
              type: array    
            type:    
              enum:    
                - MultiLineString    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON MultiLineString    
          type: object    
          x-ngsi:    
            type: GeoProperty    
        - description: Geojson reference to the item. MultiLineString    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  items:    
                    items:    
                      type: number    
                    minItems: 2    
                    type: array    
                  minItems: 4    
                  type: array    
                type: array    
              type: array    
            type:    
              enum:    
                - MultiPolygon    
              type: string    
          required:    
            - type    
            - coordinates    
          title: GeoJSON MultiPolygon    
          type: object    
          x-ngsi:    
            type: GeoProperty    
      x-ngsi:    
        type: GeoProperty    
    name:    
      description: The name of this item    
      type: string    
      x-ngsi:    
        type: Property    
    owner:    
      description: A List containing a JSON encoded sequence of characters referencing the unique Ids of the owner(s)    
      items:    
        anyOf:    
          - description: Identifier format of any NGSI entity    
            maxLength: 256    
            minLength: 1    
            pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
            type: string    
            x-ngsi:    
              type: Property    
          - description: Identifier format of any NGSI entity    
            format: uri    
            type: string    
            x-ngsi:    
              type: Property    
        description: Unique identifier of the entity    
        x-ngsi:    
          type: Property    
      type: array    
      x-ngsi:    
        type: Property    
    seeAlso:    
      description: list of uri pointing to additional resources about the item    
      oneOf:    
        - items:    
            format: uri    
            type: string    
          minItems: 1    
          type: array    
        - format: uri    
          type: string    
      x-ngsi:    
        type: Property    
    severity:    
      description: Severity of the Alarm    
      enum:    
        - informational    
        - low    
        - medium    
        - high    
        - critical    
      type: string    
      x-ngsi:    
        type: Property    
    source:    
      description: 'A sequence of characters giving the original source of the entity data as a URL. Recommended to be the fully qualified domain name of the source provider, or the URL to the source object'    
      type: string    
      x-ngsi:    
        type: Property    
    subCategory:    
      description: 'Weather categories. Enum:'' avalanches,coastalEvent, coldWave, flood, fog, forestFire, heatWave, highTemperature, hurricane, ice, lowTemperature, rainfall, rain_flood, snow, snow_ice, thunderstorms, tornado, tropicalCyclone, tsunami, wind'''    
      enum:    
        - avalanches    
        - coastalEvent    
        - coldWave    
        - flood    
        - fog    
        - forestFire    
        - heatWave    
        - highTemperature    
        - hurricane    
        - ice    
        - lowTemperature    
        - rainfall    
        - rain_flood    
        - snow    
        - snow_ice    
        - thunderstorms    
        - tornado    
        - tropicalCyclone    
        - tsunami    
        - wind    
      type: string    
      x-ngsi:    
        type: Property    
    type:    
      description: NGSI entity type. It has to be WeatherAlert    
      enum:    
        - WeatherAlert    
      type: string    
      x-ngsi:    
        type: Property    
    validFrom:    
      description: The start of the validity period for this forecast as a ISO8601 format    
      format: date-time    
      type: string    
      x-ngsi:    
        model: https://schema.org/DateTime    
        type: Property    
    validTo:    
      description: The end of the validity period for this forecast as a ISO8601 format    
      format: date-time    
      type: string    
      x-ngsi:    
        model: https://schema.org/DateTime    
        type: Property    
  required:    
    - id    
    - type    
    - alertSource    
    - category    
    - subCategory    
    - dateIssued    
  type: object    
  x-derived-from: ""    
  x-disclaimer: 'Redistribution and use in source and binary forms, with or without modification, are permitted  provided that the license conditions are met. Copyleft (c) 2023 Contributors to Smart Data Models Program'    
  x-license-url: https://github.com/smart-data-models/dataModel.Weather/blob/master/WeatherAlert/LICENSE.md    
  x-model-schema: https://smart-data-models.github.io/dataModel.Weather/WeatherAlert/schema.json    
  x-model-tags: ""    
  x-version: 0.4.1    
```  
</details>    
<!-- /60-ModelYaml -->  
<!-- 70-MiddleNotes -->  
<!-- /70-MiddleNotes -->  
<!-- 80-Examples -->  
## Ejemplo de carga útil  
#### WeatherAlert NGSI-v2 key-values Ejemplo  
Este es un ejemplo de una alerta meteorológica en formato JSON-LD como valores clave. Esto es compatible con NGSI-v2 cuando se utiliza `options=keyValues` y devuelve los datos de contexto de una entidad individual.  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "severity": "medium",  
  "category": "weather",  
  "subCategory": "snow_ice",  
  "alertSource": "http://www.meteoalarm.eu",  
  "address": {  
    "addressCountry": "ES",  
    "addressRegion": "Huesca"  
  },  
  "dateIssued": "2016-03-14T13:54:01.00Z",  
  "type": "WeatherAlert",  
  "id": "WeatherAlert-83b872975414bfca10832e564a1bb416-7",  
  "validTo": "2016-03-14T23:59:00.00Z",  
  "validFrom": "2016-03-14T13:00:00.00Z"  
}  
```  
</details>  
#### WeatherAlert NGSI-v2 normalizado Ejemplo  
He aquí un ejemplo de un WeatherAlert en formato JSON-LD normalizado. Esto es compatible con NGSI-v2 cuando no se utilizan opciones y devuelve los datos contextuales de una entidad individual.  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "WeatherAlert-83b872975414bfca10832e564a1bb416-7",  
  "type": "WeatherAlert",  
  "severity": {  
    "type": "Text",  
    "value": "medium"  
  },  
  "category": {  
    "type": "Text",  
    "value": "weather"  
  },  
  "subCategory": {  
    "type": "Text",  
    "value": "snow_ice"  
  },  
  "alertSource": {  
    "type": "Text",  
    "value": "http://www.meteoalarm.eu"  
  },  
  "address": {  
    "type": "StructuredValue",  
    "value": {  
      "addressCountry": "ES",  
      "addressRegion": "Huesca"  
    }  
  },  
  "dateIssued": {  
    "type": "DateTime",  
    "value": "2016-03-14T13:54:01.00Z"  
  },  
  "validTo": {  
    "type": "DateTime",  
    "value": "2016-03-14T23:59:00.00Z"  
  },  
  "validFrom": {  
    "type": "DateTime",  
    "value": "2016-03-14T13:00:00.00Z"  
  }  
}  
```  
</details>  
#### WeatherAlert NGSI-LD key-values Ejemplo  
Este es un ejemplo de una alerta meteorológica en formato JSON-LD como valores clave. Esto es compatible con NGSI-LD cuando se utiliza `options=keyValues` y devuelve los datos de contexto de una entidad individual.  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "WeatherAlert-83b872975414bfca10832e564a1bb416-7",  
  "type": "WeatherAlert",  
  "address": {  
    "addressCountry": "ES",  
    "addressRegion": "Huesca"  
  },  
  "alertSource": "http://www.meteoalarm.eu",  
  "category": "weather",  
  "dateIssued": "2016-03-14T13:54:01.00Z",  
  "severity": "medium",  
  "subCategory": "snow_ice",  
  "validFrom": "2016-03-14T13:00:00.00Z",  
  "validTo": "2016-03-14T23:59:00.00Z",  
  "@context": [  
    "https://raw.githubusercontent.com/smart-data-models/dataModel.Weather/master/context.jsonld"  
  ]  
}  
```  
</details>  
#### WeatherAlert NGSI-LD normalizado Ejemplo  
He aquí un ejemplo de una WeatherAlert en formato JSON-LD normalizado. Esto es compatible con NGSI-LD cuando no se utilizan opciones y devuelve los datos contextuales de una entidad individual.  
<details><summary><strong>show/hide example</strong></summary>    
```json  
{  
  "id": "uri:ngsi-ld:WeatherAlert-83b872975414bfca10832e564a1bb416-7",  
  "type": "WeatherAlert",  
  "address": {  
    "type": "Property",  
    "value": {  
      "addressCountry": "ES",  
      "addressRegion": "Huesca"  
    }  
  },  
  "alertSource": {  
    "type": "Property",  
    "value": "http://www.meteoalarm.eu"  
  },  
  "category": {  
    "type": "Property",  
    "value": "weather"  
  },  
  "dateIssued": {  
    "type": "Property",  
    "value": {  
      "@type": "DateTime",  
      "@value": "2016-03-14T13:54:01.00Z"  
    }  
  },  
  "severity": {  
    "type": "Property",  
    "value": "medium"  
  },  
  "subCategory": {  
    "type": "Property",  
    "value": "snow_ice"  
  },  
  "validFrom": {  
    "type": "Property",  
    "value": {  
      "@type": "DateTime",  
      "@value": "2016-03-14T13:00:00.00Z"  
    }  
  },  
  "validTo": {  
    "type": "Property",  
    "value": {  
      "@type": "DateTime",  
      "@value": "2016-03-14T23:59:00.00Z"  
    }  
  },  
  "@context": [  
    "https://raw.githubusercontent.com/smart-data-models/dataModel.Weather/master/context.jsonld"  
  ]  
}  
```  
</details><!-- /80-Examples -->  
<!-- 90-FooterNotes -->  
<!-- /90-FooterNotes -->  
<!-- 95-Units -->  
Consulte [FAQ 10](https://smartdatamodels.org/index.php/faqs/) para obtener una respuesta sobre cómo tratar las unidades de magnitud.  
<!-- /95-Units -->  
<!-- 97-LastFooter -->  
---  
[Smart Data Models](https://smartdatamodels.org) +++ [Contribution Manual](https://bit.ly/contribution_manual) +++ [About](https://bit.ly/Introduction_SDM)<!-- /97-LastFooter -->  
