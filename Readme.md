# K-Anonymity Data Anonymization Script

This script provides a basic implementation of k-anonymity for anonymizing a dataset. It is designed to protect sensitive information by generalizing and suppressing certain data fields.

## Features

- **Data Anonymization**: The script anonymizes a dataset by grouping data based on specific attributes and ensuring each group has at least `k` records.
- **Suppression**: Sensitive fields such as `Name`, `Postcode`, and `Patient_ID` are replaced with "Null" to prevent identification.
- **Generalization**: The `Age` field is generalized into age ranges to further protect individual identities.

## Requirements

- Python 3.x
- Pandas library
- NumPy library

## Usage

1. **Setup**: Ensure you have Python 3.x installed along with the required libraries. You can install the necessary libraries using pip:

   ```bash
   pip install pandas numpy
   ```

2. **Run the Script**: Execute the script using Python:

   ```bash
   python k_anonimity.py
   ```

3. **Output**: The script will display the original dataset and the anonymized dataset in the console.

## Parameters

- `k`: The minimum number of records required in each group for anonymization. This can be adjusted by changing the `k` parameter in the `anonymize_data` function call.

## Example

The script uses a sample dataset with patient information, including `Patient_ID`, `Name`, `Gender`, `Postcode`, `Age`, and `Disease`. It groups the data by `Disease` and `Gender`, anonymizes the data, and outputs the results.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

This script is a simple demonstration of k-anonymity and is intended for educational purposes. For more robust data anonymization, consider using specialized libraries or tools.