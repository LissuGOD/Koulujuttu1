# Koulujuttu1
classDiagram
"Person" {
  -int _id
  -string _name
  +int Id
  +string Name
  +Person()
  +Person(int id, string name)
  +string ToString()
}
"PersonCollection" {
  -List<Person> Items
  +int Count
  +void Add(Person person)
  +bool RemoveById(int id)
  +Person FindById(int id)
  +void Save(string path)
  +static PersonCollection Load(string path)
}
"Program" {
  +static void Main(string[] args)
}
"PersonCollection" --> "Person"
