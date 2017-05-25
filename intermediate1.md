Users:
{
  id: autoincrement,
  name: string,
  phone: string
}
Tables:
{
  id: autoincrement
  timeslot: time,
  open: boolean
}
Reservations
{
  name:string,
  phone: string,
  guests: integer,
  timeslot: time,
  table: integer
}

* name: String
    * Must contain only word characters
* phone: string
    * Must contain 10 digits
