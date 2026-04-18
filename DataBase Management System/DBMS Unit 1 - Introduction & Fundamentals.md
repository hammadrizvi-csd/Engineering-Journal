# 📘 DBMS - Unit 1 Notes

> Source: Handwritten Notes (Converted & Structured)  
> Reference: See original pages & diagrams :contentReference[oaicite:0]{index=0}

---

# 🔹 1. Data, Information & Database

## 📌 Data
- Raw facts (no meaning)
- Example: numbers, names, symbols

## 📌 Information
- Processed data (meaningful)
- Example: student marks report

## 📌 Database
- Organized collection of data
- Example: college student records

---

# 🔹 2. DBMS (Database Management System)

- Software that manages database

## Functions:
- Store data
- Retrieve data
- Update data
- Delete data
- Security management

## Examples:
- MySQL
- Oracle

---

# 🔹 3. Three-Level Architecture (Data Abstraction)

## 1. Physical Level (Internal Level)
- Describes how data is stored
- Includes:
  - File organization
  - Indexing
  - Compression techniques

## 2. Conceptual Level (Logical Level)
- Describes entire database structure
- Defines:
  - Tables
  - Relationships
- Used by DBA

## 3. External Level (View Level)
- User-specific view
- Shows only required data
- Example:
  - Student view
  - Teacher view

---

# 🔹 4. Data Independence

## 📌 Definition:
Ability to modify schema at one level without affecting higher level

## Types:

### 1. Physical Data Independence
- Change internal schema without affecting conceptual schema
- Example:
  - Changing storage device
  - Changing file organization

### 2. Logical Data Independence
- Change conceptual schema without affecting external schema
- Example:
  - Adding new column
  - Adding new table

---

# 🔹 5. ER Model (Entity-Relationship Model)

## 📌 Definition:
High-level conceptual model used for designing databases

---

## 🔸 Components:

### 1. Entity
- Real-world object
- Examples:
  - Student
  - Teacher
- Representation:


---

### 2. Attribute
- Properties of entity
- Examples:
  - Name
  - Roll No
- Representation:



---

### 3. Relationship
- Association between entities
- Example:
  - Student enrolls in course
- Representation:



---

# 🔹 6. Types of Attributes

## 1. Key Attribute (Primary Attribute)
- Uniquely identifies an entity
- Example: Roll No

## 2. Composite Attribute
- Can be divided into sub-parts
- Example:
  - Name → First Name + Last Name

## 3. Multivalued Attribute
- Can have multiple values
- Example:
  - Phone numbers
  - Degrees

---

# 🔹 7. Database System & Users

## 📌 Database
- Collection of logically related data

## 📌 DBMS
- Software to manage database

## 📌 Database System
- Database + DBMS + Users

---

## 👥 Types of Users:
- Naive Users
- Application Programmers
- Sophisticated Users
- DBA (Database Administrator)

---

# 🔹 8. Schema vs Instance

## Schema
- Structure of database
- Defined once

## Instance
- Actual data at a particular time
- Changes frequently

---

# 🔹 9. Keys in DBMS

## 1. Super Key
- Set of attributes that uniquely identify a record
- Example:
  - Roll No
  - (Roll No, Name)

## 2. Candidate Key
- Minimal super key

## 3. Primary Key
- Selected candidate key
- Properties:
  - Unique
  - NOT NULL

## 4. Foreign Key
- Attribute referencing another table's primary key
- Used to maintain relationship

---

# 🔹 10. Cardinality Ratio (ER Model)

## Types:

### 1. One-to-One (1:1)
- One entity → one entity

### 2. One-to-Many (1:N)
- One entity → many entities  
- Example:
  - Department → Employees

### 3. Many-to-One (N:1)
- Many entities → one entity

### 4. Many-to-Many (M:N)
- Many ↔ many  
- Example:
  - Students ↔ Courses

---

# 🔹 11. DBMS Models

| Model         | Structure        | Feature |
|--------------|-----------------|--------|
| Hierarchical | Tree            | One parent |
| Network      | Graph           | Multiple parents |
| Relational   | Table           | Most widely used |

---

# 🔹 12. Integrity Constraints

## 1. Domain Constraint
- Defines valid data type
- Example:
  - Age must be integer

## 2. Entity Integrity Constraint
- Primary key:
  - Must be unique
  - Cannot be NULL

## 3. Referential Integrity Constraint
- Foreign key must match primary key in another table
- Example:
  - Student ID must exist

---

# 🔹 13. ER Diagram Symbols

| Component     | Shape        |
|--------------|-------------|
| Entity       | Rectangle   |
| Attribute    | Ellipse     |
| Relationship | Diamond     |
| Primary Key  | Underlined  |

---

# 🔹 14. Architecture (2-Tier & 3-Tier)

## 2-Tier Architecture
## 3-Tier Architecture


---

# ✅ Summary (Quick Revision)

- Data → Raw facts  
- Information → Processed data  
- DBMS → Manage database  
- ER Model → Design database  
- Keys → Identify data  
- Constraints → Maintain accuracy  
- Architecture → System structure  

---

# 🚀 End of Unit 1
