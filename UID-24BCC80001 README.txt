UID-24BCC80001
Name- Gaganpreet Singh Bhatti
23BCC-1(B)

EXPERIMENT-1 (CODE)

1. CREATE TABLE Authors (author_id INT PRIMARY KEY, name VARCHAR(50), country VARCHAR(50));
CREATE TABLE Books (book_id INT PRIMARY KEY, title VARCHAR(100), author_id INT, FOREIGN KEY (author_id) REFERENCES Authors(author_id));
DESCRIBE Authors;
DESCRIBE Books;

2.INSERT INTO Authors VALUES (1, 'Ashish', 'India'), (2, 'Smaran', 'USA'), (3, 'Vaibhav', 'UK'); 
INSERT INTO Books VALUES (101, 'Data Science Basics', 1), (102, 'AI in Education', 2), (103, 'SQL Simplified', 1);
SELECT * FROM Authors;
SELECT * FROM Books;

3.SELECT Books.title, Authors.name, Authors.country 
FROM Books INNER JOIN Authors ON Books.author_id = Authors.author_id;
