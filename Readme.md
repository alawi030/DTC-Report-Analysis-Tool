# Manufacturer DTC Analyzer

Manufacturer DTC Analyzer is a GUI application built using Python and tkinter. It allows users to process a summary table by analyzing fault codes and generating corresponding comments based on specific rules.

## Features

- Select and browse input files, including summary table, SAE J2012DA, and manufacturer DTC files.
- Configure column indices for fault codes and starting row.
- Specify the control unit for analysis.
- Process the summary table and generate comments based on fault code analysis.
- Save the processed output to an Excel file.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/manufacturer-dtc-analyzer.git
   ```

2. Navigate to the project directory:

   ```bash
   cd manufacturer-dtc-analyzer
   ```

3. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Run the application:

   ```bash
   python main.py
   ```

2. The GUI window will appear, allowing you to interact with the application.

3. Follow the on-screen instructions to select input files, configure settings, and process the summary table.

4. The processed output will be saved as `Abgleich_herstellerspezifische_DTCs_{control_unit}.xlsx`.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please create an issue or submit a pull request.

## License

This project is licensed under the [MIT License](Licence.txt).

## Acknowledgements

The Manufacturer DTC Analyzer application was developed using Python and the tkinter library.

## Contact

For any inquiries or questions, please contact [Ali Almaliki](mailto:alawilmaliki@gmail.com).

