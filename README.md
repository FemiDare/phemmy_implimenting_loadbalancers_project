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


