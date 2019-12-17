import requests
import json

api=("https://api.exchangeratesapi.io/latest?base=")

yourCurrency=input("What currency will you exchange? ")
exchangeCurrency=input("What is your currency exchange with "+yourCurrency+ "? ")
numberofCurrency=int(input("How much"+ yourCurrency+"will you exchange? "))

result=requests.get(api+yourCurrency)
result=json.loads(result.text)
print(" 1 {0} = {1} {2}".format(yourCurrency, result["rates"][exchangeCurrency], exchangeCurrency))
print(" {0} {1}= {2} {3}".format(numberofCurrency, yourCurrency, numberofCurrency*result["rates"][exchangeCurrency], exchangeCurrency))
