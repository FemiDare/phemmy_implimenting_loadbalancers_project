# phemmy_implimenting_loadbalancers_project

I spun two EC2 instances on AWS namely "load_balance_test" and "load_balancing" also creating a keypair "load_balancing"

I then edited the inbound rules of both instances by opening port 8000 to allow traffic from anywhere 

![Screenshot 2023-11-04 114149](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/37436b6c-31a8-42be-a623-49895233f5e8)

![Screenshot 2023-11-04 115025](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/e920ef65-ddb9-4e20-9592-42a93a67e78d)

![Screenshot 2023-11-04 113905](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/3dd5adbe-7473-44b9-a64d-89d3b4fadeb5)

![Screenshot 2023-11-04 115324](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/6f49c947-0f94-4bff-a611-7d837e24d3cf)

![Screenshot 2023-11-04 115750](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/90f5af2f-a2a2-4923-b26c-911132f97b09)

![Screenshot 2023-11-04 115908](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/1f16eb93-ab10-4942-b10f-f19a6cb63309)

![Screenshot 2023-11-04 120026](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/a2194935-1762-46bd-9bf2-1f4d22c96f76)

![Screenshot 2023-11-04 120101](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/5504379f-3fa6-4c5f-9324-6622743a3c96)

I then opened two different windows on my terminal and connected to my two EC2 instances and renamed the hostnames to "firstapache" and "secondapache" respectively

I then updated my systems on both terminals and proceeded to install apache on both systems and checked the status to verify that they were both running/active

![Screenshot 2023-11-04 141154](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/c7bb3027-2141-452c-854f-c8983cf1922d)

![Screenshot 2023-11-04 141428](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/2e40a0c2-c0cc-4c58-b14a-01e213455784)

![Screenshot 2023-11-04 141701](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/15b09415-2134-4dc5-8403-070853c088a4)

![Screenshot 2023-11-04 141724](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/18b2e300-1d2a-4036-960d-bcd88a9e0edc)

![Screenshot 2023-11-04 141832](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/6dd7efe4-7a2d-428a-b71a-7fd13643b824)

![Screenshot 2023-11-04 141906](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/133ab410-0d63-4f2d-8329-5de9844b6cff)

I then proceeded to configure apache on both systems to serve content on port 8000 by adding a new "listen" directive on the port.config file

I also went to /etc/apache2/sites-available/000-default.conf on both apache systems and editted the listening port from port 80 to port 8000

I then restarted apache on both first and second systems

![Screenshot 2023-11-04 142203](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/f488d2d2-71df-47e4-8d24-80d13834e7e2)

![Screenshot 2023-11-04 153744](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/889cc634-5e64-4c5e-a0d2-8181755b3ec5)

![Screenshot 2023-11-04 142354](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/dafc8674-76c1-40af-a5cf-06a10d4f9156)

![Screenshot 2023-11-04 153853](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/a7ce5eb1-022c-458b-a20d-038cba2663e2)

![Screenshot 2023-11-04 142618](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/51d6daaa-c9c9-4b67-82d7-d5b90de71aba)

![Screenshot 2023-11-04 153926](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/a0a863c5-6a13-4001-88b2-d965ada5f68b)

![Screenshot 2023-11-04 142646](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/37fd64c6-e14e-4134-a29c-a220c4930dcc)

![Screenshot 2023-11-04 154000](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/be55ccc1-4695-4472-a8d5-e5212d4272bf)

![Screenshot 2023-11-04 142921](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/c3f7d818-6b38-43ac-9445-3dc697c41019)

![Screenshot 2023-11-04 154047](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/6515fdf0-91ed-4e31-9529-176a00f8cafa)

I opened a file named index.html on both systems

I then pasted the provided script into the file, taking sure to paste the public ip of each instance in their corresponding html file

I then changed ownership of both files and then did an override of the default html file of apache webserver

I then did a restart of apache on both systems

I ran the individual public ip on the web browser to confirm the webpage and the listening port

![Screenshot 2023-11-04 144119](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/ed2a7996-a6e6-4a5d-aba0-c7967ee37ac4)

![Screenshot 2023-11-04 154109](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/77acf4ba-8846-4700-8d8c-1199f0916c0e)

![Screenshot 2023-11-04 144341](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/9ca9f486-680a-4bf4-b81d-5b9c099812e7)

![Screenshot 2023-11-04 154209](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/9ea52aac-75c8-41f1-bba6-17d1a466c868)

![Screenshot 2023-11-04 144430](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/18fb5115-67b6-4b6b-9e65-2c1e3ce45634)

![Screenshot 2023-11-04 154242](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/ddfbcc97-a0ee-4c19-b5f0-aa552657c8a5)

![Screenshot 2023-11-04 144500](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/eaff799d-317a-43ad-9447-5071a01768ea)

![Screenshot 2023-11-04 154302](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/c9205a32-8948-4027-8937-d24ad18f6b51)

![Screenshot 2023-11-04 144541](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/d14242cf-2bbf-474d-847c-8b5983db7244)

![Screenshot 2023-11-04 154324](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/06ee731b-a35e-48fc-be98-95070fe6f72d)

![Screenshot 2023-11-04 144716](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/2d3eb7b4-c62a-4934-b405-dcd41c716085)

![Screenshot 2023-11-04 154422](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/a3ce0657-7073-4d41-9ac4-9cf476936a45)

I then launched an EC2 instance on AWS named "nginx_balance" and then editted the inbound rules to open port 80 so traffic can come from anywhere

I then opened a new terminal window and connected to this instance and changed the hostname to "nginxbalancer"

I then updated this system and then installed nginx on the system and confirmed that nginx was active/running on the system

![Screenshot 2023-11-04 152218](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/b74b37ad-fbfb-4f17-af7c-de6280471f3c)

![Screenshot 2023-11-04 152458](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/ab90f0f9-56f9-491b-a82e-c1b141de5fe1)

![Screenshot 2023-11-04 152548](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/8f3c855a-b5b3-4117-88ff-ea37b68d3478)

![Screenshot 2023-11-04 152730](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/03371ac0-ea96-4e25-9871-6be1d2bcaeb8)

![Screenshot 2023-11-04 152814](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/847f1e42-3d8d-4f48-826b-2ee337449e27)

![Screenshot 2023-11-04 153016](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/c251cffc-4d46-437e-b27e-fd8cb04e0662)

![Screenshot 2023-11-04 153101](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/0d6b9f3c-d903-493d-9b6b-0885a2927365)

I then proceeded to open the nginx configuration file "loadbalancer.conf" and pasted the provided script/commands making sure to change the stated IP to the IPs of both my previously setup apache servers

After that I proceeded to test the new configuration set and there were no errors so I then restarted nginx so as to load the new configuration

I then ran the nginx public IP on my web browser and refreshed the page severally to confirm that it is serving the webpages from my previously set up apache web servers

![Screenshot 2023-11-04 153146](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/0dc839cf-1932-41ee-bcea-ff8fd3c905a7)

![Screenshot 2023-11-04 153520](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/bca3089b-127a-4a96-9b81-ab855cdac87b)

![Screenshot 2023-11-04 154514](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/72f9d631-0e8e-422f-975d-78a59a69c780)

![Screenshot 2023-11-04 154529](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/7d8b6b17-4ff8-40d5-ab62-65456d7c50de)

![Screenshot 2023-11-04 154550](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/c21c83f8-a6e8-4c2f-ae88-dd064f2a7200)

![Screenshot 2023-11-04 154655](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/33c7a10a-40dd-458f-adb6-2acff45a92d7)

![Screenshot 2023-11-04 154820](https://github.com/FemiDare/phemmy_implimenting_loadbalancers_project/assets/140294606/b9b570ec-d4b2-4fa6-b960-644f9eb6783d)

