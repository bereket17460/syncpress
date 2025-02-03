# SyncPress

SyncPress is a Python program designed to help you keep your Windows desktop tidy by arranging desktop icons according to user-defined rules. It allows you to specify the position of each icon based on your preferences, ensuring a neat and organized desktop.

## Features

- Retrieve current positions of desktop icons.
- Arrange icons based on user-defined rules.
- Load rules from a JSON file for flexibility and easy customization.

## Installation

1. Ensure you have Python installed on your system.
2. Install the required Python packages using pip:
   ```bash
   pip install pywin32
   ```

## Usage

1. Define your rules in a `rules.json` file. The file should be in the same directory as `syncpress.py`. Here's an example of the `rules.json` format:

   ```json
   {
     "MyDocument": {"position": [100, 200]},
     "MyFolder": {"position": [300, 400]}
   }
   ```

   Each entry specifies the icon name and its desired position on the desktop.

2. Run the script using Python:

   ```bash
   python syncpress.py
   ```

3. The script will arrange the icons according to the specified rules.

## Note

- The current implementation includes a placeholder for the actual icon-moving logic. The method to set icon positions programmatically is not implemented due to limitations with Python's access to the Windows desktop environment.
- Ensure you have the necessary permissions to modify desktop items.

## Contributing

Contributions are welcome! If you have suggestions or improvements, feel free to open a pull request or issue on the GitHub repository.

## License

This project is licensed under the MIT License.