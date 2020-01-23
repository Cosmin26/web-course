# Getting started with MYSQL

## Tooling

[Download MySQL](https://dev.mysql.com/downloads/mysql/).
[Download MySQL workbench](https://dev.mysql.com/downloads/workbench/)

## Learn more

[MySQL tutorial](https://www.mysqltutorial.org/)

## Introduction to MySQL

#### Creating tables

[Learn more about MySQL data types](https://www.w3schools.com/sql/sql_datatypes.asp).

```sql
CREATE TABLE IF NOT EXISTS `people` (
  `id` INT AUTO_INCREMENT,
  `name` VARCHAR(150) NOT NULL,
  `gender` VARCHAR(6),
  `dateOfBirth` DATE,
  `address` VARCHAR(255),
  `email` VARCHAR(255),
  PRIMARY KEY (`id`) )
ENGINE = InnoDB;
```

#### Drop tables

```sql
DROP TABLE `people` ;
```

#### Insert in tables

```sql
INSERT INTO `people` (name, gender, dateOfBirth, address, email)
VALUES ("John", "Male", "1980-11-09", "Peachtree Street", "john@doe.com");
```

#### Delete from tables

```sql
DELETE FROM `people` WHERE id=1;
```

#### Selecting from tables

```sql
SELECT * FROM `people` WHERE gender = 'Male';
```

#### Ordering data

```sql
SELECT * FROM `people` WHERE gender = 'Male' ORDER BY dateOfBirth ASC
```

## Code together

#### Has one and belongs to one relationships

- Create a `people` table having: `id`, `spouseId`, `name`, `dateOfBirth` and `gender`.
- Add at least 6 people to the table.

- Select all the people having date of birth after 1990-01-01, displaying also the names of their spouse.

#### Has many and belongs to one relationships

- Create a `people` table having: `id`, `name`, `dateOfBirth` and `gender`.
- Add at least 3 people to the table.

- Create a `animals` table having: `id`, `ownerId`, `type`, `name`, `dateOfBirth`.
- Add at least 3 animals to the table.

- Select all the animals from the table and also display the name of thei owner.

#### Many to many relationships

- Create a `people` table having: `id`, `name`, `dateOfBirth` and `gender`.
- Add at least 3 people to the table.

- Create a `books` table having: `id`, `authorId`, `title`, `publishDate`.
- Add at least 3 books to the table.

- Create a `bookAuthors` table having `bookId`, `authorId`.

- Select all the authors for the book with `id=2`.

## Homework

- Create an `employees` database.
- Create a `employees` table having `id`, `name`, `dateOfBirth` and `gender`.
- Add at least 3 people to the table.

- Create a `salaries` table having `id`, `employeeId` and `amount`.
- For each `employee` create a record in the `salaries` table.
- Select all the employees having salary largen than 10000.
