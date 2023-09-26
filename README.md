# Directory Enumerator

Directory Enumerator is a simple Python script that checks the validity of directories on a web server by sending HTTP requests. It reads a list of directories from a file and checks if they exist on the target server.

**Disclaimer: Use this tool responsibly and at your own risk.**

This software is provided for educational and informational purposes only. The authors and contributors of this tool are not responsible for any misuse, damage, or legal consequences that may arise from its use. 

You are solely responsible for ensuring that your use of this tool complies with all applicable laws and regulations. This tool should only be used on systems and resources for which you have explicit permission or legal authorization.

Please review the [GPL](LICENSE) file for complete details regarding the software's licensing terms.

Always use this tool in an ethical and responsible manner, respecting the privacy and security of others. The authors disclaim any liability for misuse or unauthorized use of this tool.

By using this tool, you agree to accept all associated risks and responsibilities.


![Example run](https://raw.githubusercontent.com/onurcangnc/dir_enum/main/example_run.png)

## Prerequisites

Before running the script, make sure you have the following prerequisites installed:

- Python 3.x
- Requests library (`pip install requests`)

## Usage

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/directory-enumerator.git

2. Navigate to the project directory:
   
   ```bash
   cd directory-enumerator

3. Create a file named wordlist.txt containing the list of directories you want to check, with each directory on a separate line.

4. Run the script with the following command:
   
   ```python
   python3 directory_enumerator.py <target_url>

   Replace <target_url> with the URL of the web server you want to check.

## Example

Suppose you have a wordlist.txt file with the following content:

    
    admin
    images
    scripts
    config

Running the script with the command:

    ```python
    python directory_enumerator.py http://example.com

The script will send HTTP requests to the target server and report valid directories if they exist.

## Output

The script will print the valid directories found on the server, like this:

    
    Valid directory: http://example.com/admin
    Valid directory: http://example.com/images


## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

The Requests library: https://docs.python-requests.org/en/latest/