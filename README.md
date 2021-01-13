# log shipping with filebeat docker & spring boot

Clone the repository with 
```
git clone git@github.com:briansjavablog/log-shipping-with-filebeat-docker-spring-boot.git
```

## Building the Bank Account Serivice Image
```
cd bank-account-service
docker image build -t bank-service .
```
## Building the Config Service Image
```
cd config-service
docker image build -t config-service .
```
