# README

## Steps to Set Up and Run the Application

### 1. Export the Project to Eclipse IDE
- Open Eclipse IDE.
- Import the project:
  1. Click on `File` > `Import`.
  2. Select `Existing Maven Projects`.
  3. Browse to the location of your project and click `Finish`.

### 2. Update Database Configuration
- Navigate to the `src/main/resources` directory.
- Open the `application.properties` file.
- Update the following properties to match your database credentials:
  ```properties
  spring.datasource.url=jdbc:mysql://localhost:3306/<your_database_name>
  spring.datasource.username=<your_username>
  spring.datasource.password=<your_password>
  ```
  Replace `<your_database_name>`, `<your_username>`, and `<your_password>` with your actual database details.

### 3. Run the Application
- Navigate to `src/main/java` in Eclipse.
- Locate the main application class (annotated with `@SpringBootApplication`).
- Right-click on the class and select `Run As` > `Java Application`.

### 4. Check the Server Port
- Open the `application.properties` file in `src/main/resources`.
- Look for the property:
  ```properties
  server.port=8080
  ```
  If the port is not specified, the default port is `8080`. Update it if necessary.

### 5. Access the Application
- Open your web browser.
- Enter the following URL:
  ```
  http://localhost:<port_number>
  ```
  Replace `<port_number>` with the value from the `server.port` property.

## Thank You
This `README` serves as a guide to set up, configure, and run the application efficiently. For any issues, feel free to raise an issue on this repository.
