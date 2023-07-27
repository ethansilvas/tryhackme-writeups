
## Introduction

can think of a web app like a program that we use without installing 
    it is a program running on a remote server 

online shopping app 
    web app reads data about products from database
        info about products, customers, invoices 
    could have multiple databases 
        products db 
        customers db 
        sales db

searching for an item on an online shopping site 
    1. user enters item name and searches 
    2. web app queries products db for keyword 
    3. product db returns search results 
    4. web app formats results in user friendly way

many company offer bug bounty programs that offer rewards for anyone who discovers vulnerabilities within scope of program

![](Images/Pasted%20image%2020230726193932.png)

## Web Application Security Risks

now you want to buy an item from online store 
    1. log in to site 
    2. search for product 
    3. add to cart 
    4. specify address
    5. provide payment

these steps each have their own types of attacks: 
    login - attacker can try to discover the password using a bruteforce method 
    search - attacker can try to view unauthorized data by adding specific characters and codes to search term 
    payment - attacker would check if payment is sent in cleartext or using weak encryption

### Identification and Authentication Failure 

online system must identify and authenticate each user 

prone to many weaknesses like: 
    - brute force attacks 
    - allowing user to choose weak password 
    - storing credentials in plaintext 

### Broken Access Control

users able to see only the data they are allowed to see 

example vulnerabilities: 
    - failing to apply principle of least privilege 
    - being able to view or modify someone else's account 
    - being able to browse pages that require authentication as an unauthenticated user

### Injection 

users can insert malicious code as part of their input to forms and other text input 

cause is typically through lack of validation and sanitation

### Cryptographic Failures 

cryptography is the processes of encryption and decryption of data

encryption scrambles cleartext into ciphertext
    which should conceal the data to anyone who doesn't have the key to decrypt it 

examples of cryptographic failure: 
    - sending sensitive data in cleartext such as in HTTP requests 
    - relying on a weak cryptographic algorithm 
    - using default or weak keys for cryptographic functions 

## Practical Example of Web Application Security