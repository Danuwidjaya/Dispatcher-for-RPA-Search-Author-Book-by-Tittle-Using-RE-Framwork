# Dispatcher for RPA-Search-Author-Book-by-Title-Using-RE-Framework

This repository contains the **Dispatcher** component for the *RPA-Search-Author-Book-by-Title* project, built using UiPath's **Robotic Enterprise (RE) Framework**. The Dispatcher reads a list of book titles from an input source and uploads each title as a queue item in UiPath Orchestrator, allowing the **Performer** component to retrieve and process each item individually.

## Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Setup](#setup)
- [Usage](#usage)
- [Configuration](#configuration)
- [License](#license)

## Features

- **Queue Management**: Uploads book titles as queue items in UiPath Orchestrator for further processing.
- **Robust Error Handling**: Implements error handling and retry mechanisms via RE Framework to ensure reliable data upload.
- **Detailed Logging**: Provides logs for each step, aiding in monitoring and troubleshooting.
- **Flexible Data Input**: Configurable to use different data sources, such as CSV files or databases.

## Requirements

- **UiPath Studio**: Version 2022.4 or higher.
- **UiPath Orchestrator**: Ensure an active Orchestrator account and a queue for storing book titles.
- **Data Source**: The source of book titles, specified in `Config.xlsx`.

## Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/danuwidjaya/Dispatcher-for-RPA-Search-Author-Book-by-Title-Using-RE-Framework.git
   ```

2. **Open in UiPath Studio**:
   Open the cloned project in UiPath Studio to review and customize workflows as needed.

3. **Configure Data Source and Queue Name**:
   Update the `Config.xlsx` file with the queue name in Orchestrator and the path to the data source containing book titles.

## Usage

1. **Run the Dispatcher**:
   Execute the Dispatcher process from UiPath Studio or schedule it via Orchestrator to automatically populate the queue.

2. **Queue Processing**:
   Each book title is added to the specified queue in Orchestrator. The **Performer** component can then retrieve and process these items.

## Configuration

- **Config.xlsx**: Contains settings for data source location, queue name, and other necessary parameters.
- **Orchestrator Queue**: Ensure that a queue is created in UiPath Orchestrator and the queue name matches the one specified in `Config.xlsx`.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.



This README provides an overview, setup instructions, and key information for users looking to understand and work with the Dispatcher component of your RPA project. Adjust any specific parts to fit your project setup.
