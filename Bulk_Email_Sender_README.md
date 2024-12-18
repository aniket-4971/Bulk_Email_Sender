
# Bulk Email Sender

A simple GUI-based Python application to send bulk emails to recipients listed in a CSV file. The application uses Gmail's SMTP server and allows users to specify the email subject, body, and CSV file containing email addresses to send the email to. The status of the email sending process is displayed via a progress bar.

## Features

- Send bulk emails to multiple recipients.
- GUI interface built with `tkinter`.
- Progress bar to track email sending status.
- CSV file input, where the email addresses are extracted automatically.
- Handles SMTP connection securely using Gmail.

## Requirements

- Python 3.x
- `smtplib`
- `csv`
- `tkinter` (usually comes pre-installed with Python)
- `email.mime` (built-in Python module)

## Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/bulk-email-sender.git
   cd bulk-email-sender
   ```

2. Install any required dependencies (if needed):

   ```bash
   pip install -r requirements.txt
   ```

   *(Note: `requirements.txt` is optional here as all dependencies are part of Python's standard library.)*

## How to Use

1. **Run the script:**

   ```bash
   python bulk_email_sender.py
   ```

2. **GUI Instructions:**

   - **Subject:** Enter the subject for the email.
   - **Body:** Enter the message body of the email.
   - **CSV File:** Select a CSV file that contains a column with email addresses. The program will automatically detect the email column.
   - **Send Emails:** Click the "Send Emails" button to begin the process. The progress bar will show the email sending status.

3. **CSV File Format:**

   The CSV file should contain at least one column with email addresses. It can have other columns as well (e.g., name, phone number, etc.). The program will automatically detect the column containing emails.

   Example CSV format:

   ```
   Name, Email
   John Doe, johndoe@example.com
   Jane Smith, janesmith@example.com
   ```

4. **Gmail SMTP Settings:**

   - You will need to generate an app-specific password for your Gmail account (since direct use of your Gmail password isn't allowed).
   - Replace the placeholder password (`bxad vdag rttz fdmh`) in the script with your actual Gmail app password.

## Contributing

Feel free to fork this repository and make any changes you'd like. If you have suggestions for improvements, please open an issue or submit a pull request.

## License

This project is open source and available under the [MIT License](LICENSE).
