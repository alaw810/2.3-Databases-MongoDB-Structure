# Exercise 1 – 🧑🏻 Client-Centered View

In this exercise, the main perspective of the system is the **client**.  
Each client stores their own information as well as the history of glasses they have purchased.

## Collections

- **clients.json**
  - Fields: `_id`, `name`, `address`, `telephone`, `email`, `register_date`, `recommended_by`, `shoppings[]`.
  - `shoppings[]` is an array of subdocuments including `date`, `employee_id`, and `glasses`.
  - The `glasses` subdocument contains brand, graduation, glass color, frame type, frame color, price, and supplier reference.

- **employees.json**
  - Fields: `_id`, `name`, `email`, `position`, `telephone`.
  - Represents the optician’s staff.

- **suppliers.json**
  - Fields: `_id`, `name`, `address` (street, number, floor, door, city, postal code, country), `telephone`, `fax`, `nif`.
  - Represents glasses providers.

- **clients.validation.json**
  - JSON Schema validation that ensures `frame_type` can only be `"Rimless"`, `"Plastic"`, or `"Metallic"`.

## Diagram

The diagram illustrates the relationships between clients, suppliers, and employees, showing how purchases are recorded inside each client.

