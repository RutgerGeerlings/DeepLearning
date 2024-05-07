# Automated Age Verification - Code Execution Guide

## Prerequisites

Ensure your environment is set up with the following:
- .NET Core 3.1 SDK or later
- An IDE such as Visual Studio, VSCode (with C# extension), or JetBrains Rider

## Repository Structure

- **DataCleaning.cs**: This C# file contains all necessary methods for cleaning and preprocessing the data. It must be run first to prepare the data for the model training process.
- **Models Directory**: Each subdirectory within the Models directory corresponds to a specific model configuration. The directory naming follows the pattern `Samplesize(RBG/Grey)(number of layers)(other tweaks)`, which describes the model setup.
  - **Example**: `1000RBG3Dropout` would be a directory for a model trained on 1,000 RGB images with 3 layers, including dropout functionality.

## Running the Code

### Step 1: Data Cleaning and Preprocessing

1. Open your IDE and navigate to the `DataCleaning.cs` file.
2. Compile and run `DataCleaning.cs` to perform data cleaning and preprocessing. Ensure the output data is correctly formatted and stored for subsequent training.

### Step 2: Model Training

1. Open the IDE and navigate to the model directory of your choice.
2. Each model directory contains a `.cs` file that implements the model training process.
3. Compile and run the `.cs` file to train the model. Pay attention to the console output or any logs that provide insights into the training process and performance.

### Step 3: Model Evaluation

- After training, review the outputs generated by the model training script. This may include performance metrics and possibly visualizations (if implemented) to assess the effectiveness of the model in age prediction.

## Additional Notes

- For a detailed explanation of each model's configuration and specific tweaks, refer to the comments and documentation within each `.cs` file in the model directories.
- If you need to make modifications or enhance the model, refer to the specific `.cs` file that corresponds to the model configuration you are interested in adjusting.
