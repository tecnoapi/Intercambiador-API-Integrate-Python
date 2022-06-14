# Intercambiador-API-Integrate-Python

## Installation
```
pip install apiintercambiador
```

## Usage

```
from apiintercambiador import Apiintercambiador

ai = Apiintercambiador("token", True) # True = sandbox
```

# GET

```
result = ai.getProperties()
```

# POST

```
data = [
    {
        "fuente_origen": "1",
        "agency_id": "123",
        "propietario": "123",
        "status_id": "1",
        "status_property_id": "1",
        "cadastral_reference": "PYTHONTEST1"
    },
    {
        "fuente_origen": "1",
        "agency_id": "123",
        "propietario": "123",
        "status_id": "1",
        "status_property_id": "1",
        "cadastral_reference": "PYTHONTEST2"
    }
]
result = ai.addProperty(data)
```

# PUT

```
data = [
    {
        "_id": "000000000000aaaaaaaaaaaa",
        "fuente_origen": "1",
        "agency_id": "123",
        "propietario": "123",
        "status_id": "1",
        "status_property_id": "1",
        "cadastral_reference": "PYTHONTEST1"
    },
    {
        "_id": "000000000000bbbbbbbbbbbb",
        "fuente_origen": "1",
        "agency_id": "123",
        "propietario": "123",
        "status_id": "1",
        "status_property_id": "1",
        "cadastral_reference": "PYTHONTEST2"
    }
]
result = ai.updateProperty(data)
```

# DELETE

```
data = ["000000000000bbbbbbbbbbbb"]

result = ai.deleteProperty(data)
```