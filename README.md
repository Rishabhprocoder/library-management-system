# library-management-system
Good-looking, adaptive and powerful library management system website implemented with python package Django, using MySQL for database and materialize for web design, embedded with a lot of nice features.

# Prerequisites

MySQL

1. Install MySQL
2. Install MySQL Workbench
3. Create an empty schema named book in MySQL
4. Import /source/book.sql file into book schema via
   - Replace USERNAME with the your local instance MySQL username, which is usually root
   - Replace PATH with the actual path of /source/book.sql file
   - Input the password for your local instance MySQL afterwards

mysql -u USERNAME -p book < PATH

5. In book schema, the following tables are important:
   - auth_user stores all the users including readers, staff and superusers
   - books stores the book info
   - libraries stores the library info
   - loans stores the loan info
   - reserves stores the reservations
   - storages stores the storage info

# Library Management System

Features

1. Good-looking, neat and adaptive web design
2. Sign up, sign in, update user profile, change password, log out
3. View all the books
4. Search for a book, view book info, storage info, comments
5. Add a book, delete a book
6. Comment on a book, delete a comment
7. Loan a book
8. Return date can be extended once at most
9. Return a book
10. Reserve a book (apply for moving the book from one library to another)
11.Confirm a reservation (confirm that the book is moved to another desired library)
12. View all comments
13. View all reservations
14. View all loans
15. Django administration site available for superusers
