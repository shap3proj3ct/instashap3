# instashap3
# Instagram Account Matching Tool
Overview:

The Instagram Account Matching Tool is a Node.js script designed to identify potential ownership connections between Instagram accounts by analyzing linked email addresses and phone numbers. By examining the starting and ending characters of contact information associated with different usernames, the script helps uncover accounts that may belong to the same user.

Features:

Automated Username Scanning: The script automatically interacts with Instagram’s password reset process to retrieve linked emails or phone numbers for each username provided.
Contact Information Matching: It derives a simplified format of the email or phone number (using the first and last characters) and compares these formats across multiple accounts to find potential matches.

User-Friendly Input: The script prompts users for a file containing usernames and allows for entering a target email or phone number for comparison.

How It Works:

Input Usernames: Users provide a file containing a list of Instagram usernames.
Scan for Emails/Phone Numbers: The script scans each username to determine if there is a linked email or phone number.
Match Contact Information: If an email or phone number is found, the script extracts the first character and the last character, creating a simplified format. It checks this format against results from other usernames to identify potential matches.
Display Results: After scanning all usernames, users can enter a target email or phone number to see if any accounts matched the derived formats.
Example Use Case
For example, if the username exampleuser123 is associated with the email e*******3@gmail.com, the script derives the simplified format e3@gmail.com. It then searches through the results to identify other accounts with similar formats, such as e456@gmail.com or e123@gmail.com, indicating potential shared ownership.

Requirements:

Node.js (v14 or higher)
Puppeteer library
A file containing usernames in plain text
Installation
Create a JSON file named useragents.json containing a list of user agents to randomize the script's requests.
Clone the repository:

Copy code:

sudo apt update && apt upgrade -y
git clone https://github.com/yourusername/instagram-account-matching-tool.git
cd instashap3

Usage:
Prepare a text file (e.g., users.txt) containing Instagram usernames, one per line.

Run the script:
bash
Copy code
node instafaketest.js
Follow the prompts to enter the path to your usernames file and any target email or phone number for matching.
Contributing
Contributions are welcome! If you have suggestions for improvements or features, please create an issue or submit a pull request.
