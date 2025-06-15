# wp-all-import-POC
Step by step to POC this vulnerability<br>
<br>
Step 1: Create a valid xml file to trick the system into thinking the zip file contains valid files, so it downloads and extracts it **fake.xml**.
![XML File](https://drive.google.com/file/d/1EAxiFo_SG_zlDhspPZkQwHQQEyHjfedD/view?usp=sharing)
<br>
Step 2: Create a webshell file with the format .phar ***roll.phar*
![Web shell](https://drive.google.com/file/d/1GjcT96SngnhIls4zt8SGBF92EQOmVQtG/view?usp=sharing)
<br>
Step 3: Compress the two files fake.xml and roll.phar into one zip file **payload.zip**
![Payload.zip](https://drive.google.com/file/d/1RtiXYHXInzSvsN2togZxcJN5e-aPUoTj/view?usp=sharing)
<br>
Step 4: Upload the payload.zip file you just prepared at http://localhost/wp-admin/admin.php?page=pmxi-admin-import
![Upload success](https://drive.google.com/file/d/10qHhdddHKKLmTp701l0Hb6g7Qu3tKfel/view?usp=sharing)
<br>
Step 5: Access the returned link after a successful upload
![Access webshell](https://drive.google.com/file/d/1qpHUnoI3QjG763xIxmGD8OXVUM1Nl1CW/view?usp=sharing)

You can refer to the POC video below
![Video POC](https://drive.google.com/file/d/124s4yMJRBEblzCaYZb-nDgCzsGGsD92s/view?usp=sharing)

