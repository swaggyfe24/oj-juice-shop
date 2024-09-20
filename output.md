cd Documents/
git clone https://github.com/swaggyfe24/oj-juice-shop.git
cd oj-juice-shop
history
docker pull bkimminich/juice-shop
docker run -d -p 3000:3000 bkimminich/juice-shop
history
#Committing directly to the master branch in Github is not reccommended, commiting directly to the master increases the risk of break changes that can have a negative affect on the entire project. Also, when commiting something directly to the master and you locate a mistake it can be very difficult to revert.

#I did not make any changes to my repo settings this far at step 6.

#Steps to Reploy new image:

cd frontend/src/assets/public/images/products/
cp /Users/fe/Downloads/juicyEvilWasp.png ./apple_pressings.jpg
docker ps
docker stop 1eb8a3082be3
docker ps
cd
cd Documents
cd oj-juice-shop
docker ps -a\n
docker build -t oj-custom .
#Example response, this failed at 29/31 due to storage space issues on my personal laptop
[+] Building 931.4s (29/31)                                                                     docker:desktop-linux
 => [internal] load build definition from Dockerfile                                                            0.2s
 => => transferring dockerfile: 2.12kB                                                                          0.0s

Next steps if this had completed properly:
#run the new image
docker run -d -p 3000:3000 --name juice-shop-custom-container oj-custom

Verify changes
http://localhost:3000
