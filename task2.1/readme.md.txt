# Docker home task
## _Entering a country name and receiving a data about it._


The data you get is :
Country’s Full Name
Country’s Capital
Country’s Common Language
Country’s Currency Name
Country’s Currency rate (Base currency is EURO)
## note
By entering a wrong country name, u will get an error!!! 

## Python main libraries:

-requests
-flask
-jsonify

## API services

I used the following API services:

- [Country information](https://restcountries.eu/rest/v2/name/<country_name>?fullText=true)-
- [Currency information](http://data.fixer.io/api/latest?access_key=0f74f9e3e64cb0c2ce6ec5230dc7592d&format=1&symbols=ils)-

## BUILD AND RUN

1. open cmd
2. cd task2.1
3. docker build -t task2.1 .
4.docker run -it -d -p 5000:5000 task2.1
## OR
1. open cmd
2. docker build -t task2.1 .
3. docker-compose up -d

## Enter the country's name/ Testing

we enter the country's name by using the command

```sh
curl 127.0.0.1:5000/?name= country name
```
for example

curl 127.0.0.1:5000/?name=Israel
