# wp-all-import-POC
Step by step to POC this vulnerability<br>
<br>
Step 1: Create a valid xml file to trick the system into thinking the zip file contains valid files, so it downloads and extracts it **fake.xml**.
![XML File](https://github.com/darkroller210/wp-all-import-POC/blob/main/fake-xml-file.png)
<br>
Step 2: Create a webshell file with the format .phar ***roll.phar*
![Web shell](https://github.com/darkroller210/wp-all-import-POC/blob/main/malicious-file-phar.png)
<br>
Step 3: Compress the two files fake.xml and roll.phar into one zip file **payload.zip**
![Payload.zip](https://github.com/darkroller210/wp-all-import-POC/blob/main/compress%20payload.gif)
<br>
Step 4: Upload the payload.zip file you just prepared at http://localhost/wp-admin/admin.php?page=pmxi-admin-import
![Upload success](https://github.com/darkroller210/wp-all-import-POC/blob/main/Upload_malicious_file_via_zip_file.png)
<br>
Step 5: Access the returned link after a successful upload
![Access webshell](https://github.com/darkroller210/wp-all-import-POC/blob/main/Upload_malicious_file_via_zip_file-webshell.png)

You can refer to the POC video below
[Video POC](https://drive.google.com/file/d/124s4yMJRBEblzCaYZb-nDgCzsGGsD92s/view?usp=sharing)

