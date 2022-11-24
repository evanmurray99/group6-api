# MGO

Manitoba Gas and Oil (MGO) is an API that can be used to retrieve the selling
prices of gas and oil providers based in Manitoba. The user is required to
provide input with their requests: company, fuel type, and fuel grade.
In response, the user will receive information describing the current selling
price of fuel based on their request.

---

# Resource(s)

1. User can get a list of fuel prices from company name, fuel price and fuel grade (e.g. ESSO, premium, diesel)  
   {"results":["149.99¢", "154.99¢", "159.99¢"], "status":"OK"}

---

# Resource(s) Endpoints

| Endpoint Type | Endpoint                                          | Description         |
| ------------- | ------------------------------------------------- | ------------------- |
| GET           | `/prices/{company-name}/{fuel-type}/{fuel-grade}` | Gets the fuel price |

## Parameters

| Parameter    |   Type   | Description                                  | Example               |
| ------------ | :------: | -------------------------------------------- | --------------------- |
| company-name | `string` | The name of the organization that sells fuel | Esso, Co-op, Shell... |
| fuel-type    | `string` | The type of fuel                             | Gasoline, Diesel      |
| fuel-grade   | `string` | The quality of fuel                          | Premium, Mid, Regular |

## Smaple Requests and Responses

https://api.gas-stations.org/json?fuel-type=Gasoline&company-name=Shell&fuel-grade=Premium

```
 {
   "result":
   {
  "company-name": "Shell",
  "fuel-type": "Gasoline",
  "fuel-grade": "Premium",
  "price": "188.9¢"
   },
    "status": "OK"
 }
```
