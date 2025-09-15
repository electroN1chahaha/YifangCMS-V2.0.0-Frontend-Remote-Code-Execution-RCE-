The vulnerability arises in the webUploader method within app/api/controller/File.php
<img width="546" height="160" alt="图片" src="https://github.com/user-attachments/assets/99f1c909-45b7-4751-8f62-f6501570cd80" />
follow in c_file->webUploader.It uses the $uploadpath parameter to generate the storage directory for our uploaded files, 
which can be controlled.Then it passes the parameter into the $p_file ->webUploader method
<img width="941" height="492" alt="图片" src="https://github.com/user-attachments/assets/cbffb118-fbdd-4eca-8e57-0ed5a26d5f0a" />
follow in the $p_file->webUploader method.It requires us to pass in md5value and chunk parameters.Then generate a file
<img width="871" height="790" alt="图片" src="https://github.com/user-attachments/assets/7e53e594-9fe3-42d1-8204-9f10e2b8a582" />
After login,we access the interface and then pass in our parameters,then we got a file in public
<img width="414" height="279" alt="图片" src="https://github.com/user-attachments/assets/55c6cd9c-2e5c-4a0a-af51-3d84ab54d7c3" />
<img width="963" height="172" alt="图片" src="https://github.com/user-attachments/assets/14df0b8c-7fd1-40ba-9627-7708c8146109" />
Access this file
<img width="1906" height="974" alt="图片" src="https://github.com/user-attachments/assets/bec9abed-559a-423a-916b-298aee1c4ba3" />

