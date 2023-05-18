# Question3
Here's an example shell script that uses curl and awk to extract the Scheme Name and Asset Value fields from the given URL and save them in a CSV file.

shell
Save the above script in a file, for example, extract_data.sh. Make the script executable by running chmod +x extract_data.sh in your terminal. Then, you can execute the script by running ./extract_data.sh in the terminal.
The script uses curl to fetch the content of the URL and stores it in the DATA variable. Then, awk is used to process the data. The -F ';' flag sets the field separator as a semicolon, and {print $4 "," $5} prints the 4th field (Scheme Name) followed by a comma and the 5th field (Asset Value). The output is redirected to the OUTPUT_FILE in CSV format, with the header row being added first.

Once the script is executed, it will create a CSV file named scheme_data.csv containing the Scheme Name and Asset Value fields extracted from the provided URL.

Note: This script assumes that curl and awk are installed on your system. If they are not available, you can install them using package managers like apt-get (for Ubuntu) or brew (for macOS).
