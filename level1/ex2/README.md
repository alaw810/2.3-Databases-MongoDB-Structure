# Exercise 2 – Glasses-Centered View

In this exercise, the main perspective of the system is the **glasses**.  
Each pair of glasses stores its own information as well as the list of clients who bought it.

## Collections

- **glasses.json**
  - Fields: `_id`, `brand`, `graduation`, `glass_color`, `frame_type`, `frame_color`, `price`, `supplier_id`, `bought_by[]`.
  - `bought_by[]` is an array of subdocuments including `client_id`, `employee_id`, and `date`.
  - Each glass model is connected with one supplier and can be bought by multiple clients.

- **clients.json**
  - Fields: `_id`, `name`, `address`, `telephone`, `email`, `register_date`.
  - Represents the optician’s customers.

- **employees.json**
  - Fields: `_id`, `name`, `email`, `position`, `telephone`.
  - Represents the optician’s staff.

- **suppliers.json**
  - Fields: `_id`, `name`, `address` (street, number, floor, door, city, postal code, country), `telephone`, `fax`, `nif`.
  - Represents glasses providers.

- **glasses.validation.json**
  - JSON Schema validation that ensures `frame_type` can only be `"Rimless"`, `"Plastic"`, or `"Metallic"`.

## Diagram

The diagram illustrates the relationships between glasses, suppliers, employees, and clients, showing how purchases are recorded inside each glass model.

