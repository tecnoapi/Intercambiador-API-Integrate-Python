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
        "fuente_origen"=> "1123123",
         "agency_id"=> "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0aW1lIjoiV2VkIEp1biAwOCAyMDIyIDEwOjM5OjE2IEdNVCswMjAwIChob3JhIGRlIHZlcmFubyBkZSBFdXJvcGEgY2VudHJhbCkiLCJ1c2VySWQiOiI2Mjk0YmM3ZGU1ODVlODhiODYxNzYzZDAiLCJpYXQiOjE2NTQ2Nzc1NTZ9.0xFLIf631G7PbXEL_ef04O3w6gjnu8lZ-gExsR9Wfto",
         "reference"=> "11905-OB",
         "status_id"=> "1",
         "status_property_id"=> "1",
         "property_type_id"=> "8",
         "property_subtype_id"=> "2",
         "visibility_type_id"=> "2",
         "cadastral_reference"=> "9015608DF2891E0017AL",
         "price_sale"=> null,
         "price_rent"=> 95,
         "community_costs"=> "",
         "ibi_costs"=> "",
         "traspass"=> "",
         "orientation_id"=> "6",
         "energy_clasification_id"=> "6",
         "co2_release_class_id"=> "2",
         "conservation_state_id"=> "4",
    },
    {
        "fuente_origen"=> "1123123",
         "agency_id"=> "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0aW1lIjoiV2VkIEp1biAwOCAyMDIyIDEwOjM5OjE2IEdNVCswMjAwIChob3JhIGRlIHZlcmFubyBkZSBFdXJvcGEgY2VudHJhbCkiLCJ1c2VySWQiOiI2Mjk0YmM3ZGU1ODVlODhiODYxNzYzZDAiLCJpYXQiOjE2NTQ2Nzc1NTZ9.0xFLIf631G7PbXEL_ef04O3w6gjnu8lZ-gExsR9Wfto",
         "reference"=> "11906-OB",
         "status_id"=> "1",
         "status_property_id"=> "1",
         "property_type_id"=> "8",
         "property_subtype_id"=> "2",
         "visibility_type_id"=> "2",
         "cadastral_reference"=> "9015608DF2891E0018AL",
         "price_sale"=> null,
         "price_rent"=> 195,
         "community_costs"=> "",
         "ibi_costs"=> "",
         "traspass"=> "",
         "orientation_id"=> "6",
         "energy_clasification_id"=> "6",
         "co2_release_class_id"=> "2",
         "conservation_state_id"=> "4",
    }
]
result = ai.addProperty(data)
```

# PUT

```
data = [
    {
        "property_id"=> "62aafcb53e575f7b21a16dfd",
        "fuente_origen"=> "1123123",
         "agency_id"=> "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0aW1lIjoiV2VkIEp1biAwOCAyMDIyIDEwOjM5OjE2IEdNVCswMjAwIChob3JhIGRlIHZlcmFubyBkZSBFdXJvcGEgY2VudHJhbCkiLCJ1c2VySWQiOiI2Mjk0YmM3ZGU1ODVlODhiODYxNzYzZDAiLCJpYXQiOjE2NTQ2Nzc1NTZ9.0xFLIf631G7PbXEL_ef04O3w6gjnu8lZ-gExsR9Wfto",
         "reference"=> "11905-OB",
         "status_id"=> "1",
         "status_property_id"=> "1",
         "property_type_id"=> "8",
         "property_subtype_id"=> "2",
         "visibility_type_id"=> "2",
         "cadastral_reference"=> "9015608DF2891E0017AL",
         "price_sale"=> null,
         "price_rent"=> 95,
         "community_costs"=> "",
         "ibi_costs"=> "",
         "traspass"=> "",
         "orientation_id"=> "6",
         "energy_clasification_id"=> "6",
         "co2_release_class_id"=> "2",
         "conservation_state_id"=> "4",
    },
    {
        "property_id"=> "62aafcb53e575f7b21a16dfe",
        "fuente_origen"=> "1123123",
         "agency_id"=> "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0aW1lIjoiV2VkIEp1biAwOCAyMDIyIDEwOjM5OjE2IEdNVCswMjAwIChob3JhIGRlIHZlcmFubyBkZSBFdXJvcGEgY2VudHJhbCkiLCJ1c2VySWQiOiI2Mjk0YmM3ZGU1ODVlODhiODYxNzYzZDAiLCJpYXQiOjE2NTQ2Nzc1NTZ9.0xFLIf631G7PbXEL_ef04O3w6gjnu8lZ-gExsR9Wfto",
         "reference"=> "11906-OB",
         "status_id"=> "1",
         "status_property_id"=> "1",
         "property_type_id"=> "8",
         "property_subtype_id"=> "2",
         "visibility_type_id"=> "2",
         "cadastral_reference"=> "9015608DF2891E0018AL",
         "price_sale"=> null,
         "price_rent"=> 195,
         "community_costs"=> "",
         "ibi_costs"=> "",
         "traspass"=> "",
         "orientation_id"=> "6",
         "energy_clasification_id"=> "6",
         "co2_release_class_id"=> "2",
         "conservation_state_id"=> "4",
    }
]
result = ai.updateProperty(data)
```

# DELETE

```
data = ["62aafcb53e575f7b21a16dfd"]

result = ai.deleteProperty(data)
```