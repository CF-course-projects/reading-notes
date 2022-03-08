# Web App Security

## Many to many relationships

Many to many:
- Ex: a given employee can be assigned to multiple projects and a project may have multiple employees working on it
- This is done by creating employee and project tables
- Then creating an employee_project join table with employee_id and project_id as foreign keys

Model Classes:
- Model classes need to be annotated with JPA 
- Bidirectional: When both classes refer to each other
- In order to map a many to many association we use the @ManyToMany, @JoinTable and @JoinColumn annotations.
- This association has two sides:
  - The owning side: This is specified by using the @JoinTable annotation. @JoinTable is used to define the join/link table.
  - The inverse side: The @JoinColumn annotation is used to specify the join/linking column with the main table.

