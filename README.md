
# Resource(s) Endpoints


| Endpoint Type | Endpoint | Description |
| ----------- | ----------- | ----------- |
| GET | `/prices/{company-name}/{fuel-type}/{fuel-grade}` | Gets the fuel price |

## Parameters 

| Parameter   | Type        | Description | Example     |
| ----------- | :-----------: | ----------- | ----------- |
| company-name | `string` | The name of the organization that sells fuel | Esso, Co-op, Shell... |
| fuel-type | `string` | The type of fuel | Gasoline, Diesel | 
| fuel-grade| `string` | The quality of fuel | Premium, Mid, Regular |
