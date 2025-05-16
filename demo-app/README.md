# Jenkins Demo Application

This is a simple demo application designed to showcase Jenkins CI/CD capabilities. It consists of a basic HTML application with a counter feature, perfect for demonstrating various Jenkins pipeline concepts.

## Application Structure

- `index.html`: The main application file containing a simple counter with increment, decrement, and reset functionality
- `Jenkinsfile`: Defines the CI/CD pipeline for the application
- `README.md`: This documentation file

## Features

- Simple counter application with a modern UI
- Responsive design
- Interactive buttons with hover effects
- Animated counter display
- Information section about the demo

## Jenkins Pipeline Stages

The `Jenkinsfile` demonstrates several key CI/CD concepts:

1. **Checkout**: Retrieves the source code from version control
2. **Test**: Performs basic HTML validation
3. **Build**: Creates a build directory and copies necessary files
4. **Deploy**: Simulates deployment by creating a deployment log

## How to Use This Demo

1. **Set up Jenkins**:
   - Make sure Jenkins is running (using the provided docker-compose setup)
   - Access Jenkins at http://localhost:8080

2. **Create a New Pipeline**:
   - Click "New Item" in Jenkins
   - Enter a name for your pipeline (e.g., "demo-app")
   - Select "Pipeline"
   - Click OK

3. **Configure the Pipeline**:
   - In the pipeline configuration, select "Pipeline script from SCM"
   - Choose your SCM (e.g., Git)
   - Enter your repository URL
   - Specify the branch (e.g., main)
   - Set the script path to "demo-app/Jenkinsfile"
   - Save the configuration

4. **Run the Pipeline**:
   - Click "Build Now" to start the pipeline
   - Watch the pipeline progress through each stage
   - View the console output for detailed information

## Learning Points

This demo helps understand:
- Basic Jenkins pipeline structure
- CI/CD concepts (Continuous Integration/Continuous Deployment)
- Pipeline stages (Checkout, Test, Build, Deploy)
- Artifact archiving
- Pipeline success/failure handling

## Customization

Feel free to modify the application or pipeline to demonstrate additional concepts:
- Add more complex testing
- Implement actual deployment steps
- Add environment-specific configurations
- Include code quality checks
- Add notification steps 