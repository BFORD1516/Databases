What is PostgreSQL?

PostgreSQL is an advanced, open-source relational database management system (RDBMS). It supports SQL for relational queries and has extensive support for JSON and other non-relational data types. It is known for its strong standards compliance, extensibility, and support for complex queries and transactions.
What is the difference between SQL and PostgreSQL?

    SQL (Structured Query Language): SQL is a standard language used for querying and managing databases. It is used to perform tasks such as querying data, updating records, and managing database schema.
    PostgreSQL: PostgreSQL is a specific implementation of an RDBMS that uses SQL as its query language. It offers additional features beyond the standard SQL, such as support for custom data types, advanced indexing, and full-text search.

In psql, how do you connect to a database?

To connect to a database in psql, you can use the following command:
psql -h hostname -p port -U username -d database_name

Alternatively, if you have environment variables set or are connecting to a local database, you can simplify it to:
psql -d database_name

What is the difference between HAVING and WHERE?

    WHERE: The WHERE clause is used to filter rows before any groupings are made. It is applied to individual rows.
    HAVING: The HAVING clause is used to filter groups after the GROUP BY clause has been applied. It is applied to aggregated results.

What is the difference between an INNER and OUTER join?

    INNER JOIN: Returns only the rows that have matching values in both tables.
    OUTER JOIN: Returns all rows from one table and the matched rows from the second table. If there is no match, the result is NULL on the side of the table without a match. Outer joins can be further divided into LEFT OUTER JOIN, RIGHT OUTER JOIN, and FULL OUTER JOIN.

What is the difference between a LEFT OUTER and RIGHT OUTER join?

    LEFT OUTER JOIN: Returns all rows from the left table and the matched rows from the right table. If no match is found, NULLs are returned for columns from the right table.
    RIGHT OUTER JOIN: Returns all rows from the right table and the matched rows from the left table. If no match is found, NULLs are returned for columns from the left table.

What is an ORM? What do they do?

ORM stands for Object-Relational Mapping. It is a programming technique used to convert data between incompatible type systems in object-oriented programming languages. ORMs allow developers to interact with a database using the programming language's objects rather than SQL queries. Examples include Django ORM for Python, Hibernate for Java, and Entity Framework for .NET.
What are some differences between making HTTP requests using AJAX and from the server side using a library like requests?

    AJAX:
        Runs in the browser, enabling asynchronous web requests without reloading the page.
        Useful for dynamic, interactive web applications.
        Limited by the same-origin policy (unless CORS is implemented).

    Server-side (e.g., using requests in Python):
        Runs on the server, suitable for backend operations.
        Not restricted by the same-origin policy, so can make requests to any endpoint.
        Typically used for tasks like API integrations, web scraping, and server-to-server communication.

What is CSRF? What is the purpose of the CSRF token?

CSRF (Cross-Site Request Forgery) is a type of attack that tricks the user into submitting a malicious request. It exploits the user's authenticated session to perform actions without their consent. The CSRF token is a unique, secret value sent with each request to verify that the request is genuine and originated from the authenticated user. This helps protect against CSRF attacks by ensuring that the request is intentional and not forged.
What is the purpose of form.hidden_tag()?

In web frameworks like Flask-WTF (Flask with WTForms), form.hidden_tag() is used to render hidden fields required for form submission. It often includes CSRF tokens and other metadata necessary for form validation and security. This ensures that hidden fields are included in the form and helps protect against CSRF attacks.
