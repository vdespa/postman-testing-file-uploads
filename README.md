# postman-testing-file-uploads
A sample postman collection showing how you can tests 


## Getting started

1. Add the files you want to upload to the same folder where this readme is located.
2. Edit the data.csv file and change the file names. file1.txt is provided as a sample
3. Edit the collection, make sure the address and the endpoint are right. Also check that the parameter is file.
4. Run the collection

a. with Newman installed locally
    `newman run collection.json --iteration-data data.csv`

b. with Docker
    `docker run -v $PWD:/etc/newman -t postman/newman_ubuntu1404 run collection.json --iteration-data data.csv`
  
