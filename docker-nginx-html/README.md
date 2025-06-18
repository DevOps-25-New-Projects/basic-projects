✅ Step-by-Step Instructions
🔹 Step 1: Start an Ubuntu container with port mapping

docker run -it -p 8080:80 ubuntu bash

This runs a new Ubuntu container interactively and maps host port 8080 to container port 80 (Nginx default).

🔹 Step 2: Update package lists

Inside the container, run:

apt update
🔹 Step 3: Install nginx and nano

apt install -y nginx nano

nginx is the web server.
nano is a simple text editor to create the HTML file.

🔹 Step 4: Create your HTML file

Navigate to the default HTML folder:

cd /var/www/html
Create a file called index.html:

nano index.html

Paste this index.html file content here

Save with Ctrl + O, press Enter, then Ctrl + X to exit.

🔹 Step 5: Start the Nginx service

service nginx start
🔹 Step 6: Test it in your browser

Open your browser and go to:

http://localhost:8080
You should see the HTML page you just created.



