# Spatpy: Spatial Transcriptomics Analysis Tool

## Overview
**Spatpy** is a software tool designed for spatial transcriptomics analysis. It focuses on tasks such as cell segmentation, annotation, and slice alignment. This tool provides an interactive web interface for users to easily manage and visualize spatial transcriptomics data, making it a powerful resource for bioinformatics researchers working with spatial data.

## Features
- **Cell Segmentation**: Automatically segments cells based on spatial data.
- **Annotation**: Annotates segmented cells with relevant biological information.
- **Slice Alignment**: Helps in aligning tissue slices for accurate analysis.
- **Interactive Web Interface**: Built with Dash, providing an intuitive and user-friendly experience.
  
## Installation

### 1. Install Dependencies
To run **Spatpy**, you need to set up a Conda environment using the provided `environment.yml` file. This will ensure that all required dependencies are installed in an isolated environment.

1. Clone or download the project repository.
2. In the project directory, create a Conda environment by running:
    
    ```
    conda env create -f environment.yml
3. Activate the environment:
   
    ```
   conda activate Spatpy
### 2. Additional Dependencies
If you prefer to manually install dependencies or need additional packages, you can install them using:

    conda install <package_name>
## Running the Application

Once the environment is set up, you can run the web application using the following steps:

1. Navigate to the project directory (where the `main.py` file is located).
2. Run the app with custom parameters (host, port, debug mode) by executing the following command:

   ```bash
   python main.py --host <host_address> --port <port_number> --debug <True/False> --use_reloader <True/False>
   ```

   For example, to run the app on `127.0.0.1` at port `8088`:

   ```bash
   python main.py --host 127.0.0.1 --port 8088
   ```

3. Once the app is running, open your web browser and navigate to:

   ```
   http://127.0.0.1:8088
   ```

   You should now see the Spatpy interface.

## Customization
You can configure various aspects of the application by modifying the provided `main.py` file. The Dash framework allows for easy integration of client-side callbacks, layout customization, and error handling. For instance, error handling is managed through the `global_error_handler`, and user interactions are captured via JavaScript event listeners.

## License
Spatpy is open-source and licensed under the MIT License.

## Contact
For any issues or contributions, please contact us at: [ybzhou@seu.edu.cn](ybzhou@seu.edu.cn)