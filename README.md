# MGO

Manitoba Gas and Oil (MGO) is an API that can be used to retrieve the selling
prices of gas and oil providers based in Manitoba. The user would need to
provide input with their requests: company, fuel type, and fuel grade.
In response, the user will receive information describing the current selling
price based on their request.

---

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
