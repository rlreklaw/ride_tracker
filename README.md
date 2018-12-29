# Spring JDBC Pluralsight course

## General Notes
* https://app.pluralsight.com/library/courses/building-applications-spring-jdbc/table-of-contents
* Use MySQL workbench to create `ride_tracker` schema and `ride` table
* Often have to run the JUnit tests twice to get them to succeed.  They usually timeout and fail when run the first time after the server is started.  Success on the second attempt.

For batch update demo we added a `ride_date` column to the table
	`alter table ride add ride_date datetime after duration;`
	
`batchUpdate()` works for both `insert` and `update` statements.

also use the `jdbcTemplate.update()` method to run `delete` SQL statements
