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

