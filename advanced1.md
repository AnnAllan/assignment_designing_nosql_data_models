Products
{
    id: autoincrement,
    name: string,
    description: text,
    product_cost: float,
    price: float,
    sku: string,
    department_id: integer,
    inventory: integer
}
Stock
{
  product_id: integer,
  name: string,
  sku: string,
  department: string,
  inventory: integer
}
Receipts
{
  id: autoincrement,
  date: datetime,
  customer_name: string,
  billing_address: text,
  shipping_address: text,
  product_list: array[product_id],
  total_cost: float,
  payment_method: string
}
Revenue
{
  product_id: integer
  product_cost: float,
  price: float,
}

* sku: String
    * Must be unique
* password: String
    * Must be at least 8 characters
