# geocode-google
Geocode addresses with Google API from a CSV file

2016 First written by shanealynn https://github.com/shanealynn
2018 Forked and modified for better use and modern Google API by TannerCrook https://github.com/TannerCrook

This script will geocode addresses that are in a csv file. The script has a variable for the address search string column name
so you can adjust to whatever the column header is. The output will be put into the file specified in the ouput_filename variable.

Your csv can contain other data but it will not be put to the output file, so make sure you use the input string as a key or keep the
ordering the same.

After every 500 successul geocode operations, a temporary file with results is recorded in case of 
script failure / loss of connection later.

Addresses and data are held in memory, so this script may need to be adjusted to process files line
by line if you are processing millions of entries.

Big thanks to @shanealynn for saving me time not having to write all the basics. 
