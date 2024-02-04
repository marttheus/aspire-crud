
░█████╗░░██████╗██████╗░██╗██████╗░███████╗
██╔══██╗██╔════╝██╔══██╗██║██╔══██╗██╔════╝
███████║╚█████╗░██████╔╝██║██████╔╝█████╗░░
██╔══██║░╚═══██╗██╔═══╝░██║██╔══██╗██╔══╝░░
██║░░██║██████╔╝██║░░░░░██║██║░░██║███████╗
╚═╝░░╚═╝╚═════╝░╚═╝░░░░░╚═╝╚═╝░░╚═╝╚══════╝

## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Create:** Add new items to the database.
- **Read:** Retrieve and display information from the database.
- **Search:** Retrieve and display paginated information from the database.
- **Update:** Modify existing records in the database.
- **Delete:** Remove items from the database.

## Getting Started

### Prerequisites

- [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0) installed
- Aspire Workload installed
    ```console
    dotnet workload update
    dotnet worload install aspire
    ```
- PostgreSQL

### Installation

1. Clone the repository:

    ```console
    git clone https://github.com/marttheus/aspire-crud.git
    ```

2. Navigate to the project directory:

    ```console
    cd aspire-crud
    ```

3. Restore dependencies:
    ```console
    dotnet restore
    ```

### Configuration

1. Open the appsettings.json file and update the database connection string.
    ```json
    {
      "ConnectionStrings": {
        "DefaultConnection": "YOUR_DATABASE_CONNECTION_STRING"
      }
    }
    ```

2. Apply database migrations:
    ```console
    dotnet ef database update
    ```

## Usage

1. Build and run the application:

    ```console
    dotnet build
    dotnet run
    ```

2. Access the API at http://localhost:5000 or https://localhost:5001 in your preferred API testing tool (e.g., Postman).

3. Use the API to perform CRUD operations on entities.

## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.