# imsr_dataframe_creation_and_update_program

This program reads all the PDF files from a specified folder and extracts the required data from them into a pandas DataFrame. It defines a list of columns for the DataFrame, initializes an empty DataFrame, and defines a function that extracts data from a PDF file and appends it to the DataFrame.

The process_pdf() function uses the PyMuPDF library to open the PDF file and extract text from all pages. It then uses regular expressions to extract specific data from the text, such as the date, national preparedness level, initial attack activity, new large incidents, large fires contained, uncontained large fires, area command teams committed, NIMOs committed, Type 1 IMTs committed, Type 2 IMTs committed, and Complex IMTs committed.

After extracting the data, the function creates a new DataFrame from the extracted data and appends it to the existing DataFrame using the concat() function. The process_pdf() function is called for all PDF files in the specified folder using the os.listdir() function
