# AUTOMATED-REPORT-GENERATION

COMPANY: COOTECH IT SOLUTIONS

NANE: sharan ganesh konakala

INTERN ID: CT06DN445

DONAIN: Python Programming

DURATION: 6 WEEEKS

MENTOR: NEELA SANTOSH

DESCRIPTION

This Python script is designed to generate a detailed sales report in PDF format by reading data from a CSV file, processing it, and then formatting the results into a well-structured and professional document. To accomplish this, the script uses two key libraries: the built-in csv module and the third-party fpdf library. The csv module is essential for reading and parsing the CSV file named data.csv. This file contains sales data with columns such as "Name" and "Sales". Using the csv.DictReader class, each row of the CSV is read into a dictionary format, allowing the script to access data by column headers efficiently. One notable aspect of the dataprocessing is the conversion of the "Sales" figures from strings with currency symbols and formatting—such as "$1,200.00"—into floating-point numbers. This is necessary because the raw sales data contains characters like dollar signs and commas which prevent direct numerical operations. The script removes these characters using string replacement methods before converting the cleaned strings into floats. This conversion allows subsequent calculations to be performed accurately.

Once the data is loaded and cleaned, the script proceeds to compute several summary statistics that are essential for the sales report. It calculates the total sales bysumming all individual sales values, the average sales by dividing this total by the number of sales entries, and determines the highest single sale from the dataset. Additionally, it identifies the top seller—the person with the highest sales—by using Python's max() function combined with a lambda function to extract the salesperson's name associated with the maximum sale. These summary values provide meaningful insights into the sales performance and are included in the final report.

The generation of the PDF report is handled by the fpdf library, which is a popular and lightweight tool for creating PDF files programmatically in Python. The script beginsby creating an instance of the FPDF class and adding a new page. It then sets the font style and size to Arial Bold with a size of 16 points to display a centered title, “Sales Report,” prominently at the top of the page. After a line break, the script creates a table to present the individual sales data. The table headers “Name” and “Sales” are printed in bold font with borders for clear separation. For each row of data, the salesperson’s name and their sales figure are printed, with the sales value formatted back into a currency string (including commas and the dollar sign) for readability. The table rows are separated by borders, which visually organize the data.
Following the detailed sales table, the script adds a summary section with the calculated total sales, average sales, highest sale, and top seller’s name. The font is adjusted to Arial Bold at size 14 for the “Summary” heading and regular font at size 12 for the summary details, ensuring clear visual hierarchy. Each summary statistic is printed on a new line for clarity.

Finally, the script saves the entire report as a PDF file named report.pdf on the local disk and prints a confirmation message to indicate successful generation. This script is practical for anyone needing automated report creation from raw sales data, and it demonstrates the combined use of Python’s standard library andan external PDF generation package to handle data reading, processing, and formatted output creation. The modularity and simplicity of the code allow easy customization for different datasets or report formats, making it a versatile tool for generating professional sales reports quickly and efficiently.

OUTPUT

![Image](https://github.com/user-attachments/assets/ceb77296-5b23-45f6-a877-1a4024d607b7)
