Students
{
  id: autoincrement,
  username: string,
  password: string,
  class: string,
  examGrade: string,
}
Semester
{
  id: autoincrement,
  class: string,
  student_id: string
}
* username: String
    * Must contain only word characters
* password: String
    * Must be at least 8 characters
