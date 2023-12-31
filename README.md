# Your Go Application

This is a simple Go application that does iCalendar files (.ics) analyzes and sends notifications by email based on the events in these iCalendar files.

## Prerequisites

Before you begin, ensure you have the following installed:

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Getting Started

1. **Clone the repository:**

    ```bash
    git clone <repository-url>
    ```

2. **Create an environment variables file:**

   Create a file named `.env` in your project directory. Fill this file with the required environment variables:

    ```env
    FROM_EMAIL=user@example.com
    TO_EMAIL=recipient@example.com
    EMAIL_PASSWORD=your_password
    SMTP_HOST=smtp.example.com
    SMTP_PORT=587
    ICS_DIR=/path/to/ics/files
    ```

   Customize the values according to your application.

3. **Build and run the Docker container:**

    ```bash
    docker-compose up --build
    ```

   This command uses Docker Compose to build and run the container, loading environment variables from the `.env` file.

4. **Access your application:**

   Open your web browser and go to [http://localhost:8080](http://localhost:8080).

## Customizing the Docker Image

- If your application uses additional environment variables, add them to the `.env` file.
- Customize the Dockerfile or docker-compose.yml if needed.

## Contributing

If you'd like to contribute, please fork the repository and create a pull request. Feel free to open an issue if you encounter any problems or have suggestions.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
