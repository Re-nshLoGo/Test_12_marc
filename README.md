# Post API with MySQL and AWS deployment demo
  This is a simple Java-based API that uses MySQL to store data. 
  It allows users to add new posts and retrieve a list of all posts.
  
 ## API Endpoints
  This API has the following endpoints:

 * GET /posts -
 Returns a list of all posts.

* POST /posts -
Adds a new post.

 * Request Body -
The request body should be a JSON object with the following fields:
      * title (required) - The title of the post.
      * description (required) - The description of the post.
 * Response Body
    The response body will be a JSON object with the following fields:

    * id - The ID of the newly created post.
    * title - The title of the post.
    * description - The description
  
 ## To configure the API using a properties file: -
  * Add the following properties to the file:
       * spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
       * spring.datasource.url = jdbc:mysql://localhost:3306/test_db
       * spring.datasource.username = root
       * spring.datasource.password = password
       * spring.jpa.show-sql = true
       * spring.jpa.hibernate.ddl-auto = update
       * spring.jpa.properties.hibernate.dialect = org.hibernate.dialect.MySQL5Dialect
