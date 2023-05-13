# TicketGenerator


This code reads data from a CSV file containing the registration details of teams participating in an event, and generates a ticket for each team. The ticket includes a QR code with the team details and an event logo. The team name, category, members, and contact information are also displayed on the ticket along with the Think Tank and MLSA logos.

The code first imports the necessary modules, including csv for reading the CSV file, qrcode for generating the QR code, and PIL for creating and editing the ticket image. It then opens the CSV file and uses csv.DictReader to read each row as a dictionary.

For each row, the code extracts the relevant data, creates a string with the event details, generates a QR code from the string, and resizes the QR code to fit the ticket. It then creates a blank ticket image, adds the event logo and QR code to the ticket, and adds the team details and logos to the ticket. If the team is participating in a programming language-specific category, the code also adds the logo of the programming language to the ticket.

Finally, the code saves each ticket image as a PNG file.
