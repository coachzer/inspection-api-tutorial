# Learning .NET 6 Web API with Entity Framework Core and SQL Server

This repository contains a project that focuses on learning how to build a Web API using .NET 6, Entity Framework Core, and SQL Server. The goal of the project is to create an inspection system for floor buildings, allowing users to manage and track the status of each inspection (e.g., First Floor, Second Floor, Mezzanine). Inspections can be categorized as either satisfactory (SAT) or unsatisfactory (UNSAT), and users can leave comments related to each inspection. The application provides functionality to add, update, and delete inspections.

## Technologies Used

- .NET 6: The .NET framework version used for the application.
- Swagger UI: Building a RESTful API for handling HTTP requests and responses.
- Entity Framework Core: Object-relational mapper for working with databases.
- SQL Server: A relational database management system for data storage.
- C#: The programming language used for developing the application.

## Getting Started

To run the project locally, follow these steps:

1. Clone the repository: `git clone https://github.com/your-username/your-repository.git`
2. Navigate to the project directory: `cd your-repository`
3. Install dependencies: `dotnet restore`
4. Configure the database connection string in the `appsettings.json` file.
5. Run database migrations: `dotnet ef database update`
6. Start the application: `dotnet run`
7. Access the API at: `http://localhost:4200`- as we used Angular for the frontend

## API Endpoints

The API provides the following endpoints:

- **Inspections**:
  - `GET /api/inspections`: Retrieve a list of all inspections and their details.
  - `GET /api/inspections/{id}`: Retrieve the details of a specific inspection.
  - `POST /api/inspections`: Create a new inspection.
  - `PUT /api/inspections/{id}`: Update the details of an existing inspection.
  - `DELETE /api/inspections/{id}`: Delete an inspection.

- **Inspection Types**:
  - `GET /api/inspectionTypes`: Retrieve a list of all inspection types.
  - `GET /api/inspectionTypes/{id}`: Retrieve the details of a specific inspection type.
  - `POST /api/inspectionTypes`: Create a new inspection type.
  - `PUT /api/inspectionTypes/{id}`: Update the details of an existing inspection type.
  - `DELETE /api/inspectionTypes/{id}`: Delete an inspection type.

- **Status**:
  - `GET /api/status`: Retrieve a list of all inspection statuses.
  - `GET /api/status/{id}`: Retrieve the details of a specific inspection status.
  - `POST /api/status`: Create a new inspection status.
  - `PUT /api/status/{id}`: Update the details of an existing inspection status.
  - `DELETE /api/status/{id}`: Delete an inspection status.

## Future Enhancements

This project serves as a starting point for learning .NET 6 Web API development. Some potential enhancements that can be implemented in the future include:

- Authentication and authorization for secure access to the API.
- Improved error handling and validation.
- Pagination and sorting options for retrieving inspections.
- Implementing search functionality for finding specific inspections.
- Adding unit tests to ensure the stability of the application.

## Contributing

Contributions to this project are welcome. If you have any ideas or improvements, please feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use and modify the code as per the terms of the license.

## Acknowledgements

This project was created as a part of the learning process for .NET 6 Web API development and was done by following [this tutorial](https://youtu.be/rzPFEuKlPhM).
