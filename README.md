# Pro Direct ATC Guide
## Commands List:
- ```?pds URL/PID``` *This will scrape all SKU's for the desired link/pid regardless of Elite+ or not.*
- ```?setcookie``` *Use this command to set your cookie, usage explained below. Cookie stays until banned.*
- ```?atc PID SKU``` *Use this command to initiate the ATC. Must send the* **PID** *with* **SKU** *seperated by a* **SPACE**

## Usage
> First acquire your account/akamai cookies:
- Login to PD and get a [dummy product](https://www.prodirectsoccer.com/p/pug-206705/)
- Open your network logs (**F12**) and click the **Network Tab** and select **Fetch/XHR**
- Add the product to your cart and look for the request named **addbasketline** and copy it as a **NODEJS Fetch** as show below.


![Get Cookies](https://i.ibb.co/nMS2f0b/Screenshot-10.png)


> Send the cookie to the bot.
- Send your clipboard to the bot with the command ```?setcookie``` it is fine if it sends it as a txt file or as text it can parse both.
- The bot should set your cookie and keep it assigned to your discord until it becomes banned. *(Only allows a few ATC requests)*
- Clear your cart once done to ensure a faster checkout afterwards.
- If the bot has successfully gathered all cookies it will return a message like so.


![Success Cookie](https://i.ibb.co/RTmjxFy/Screenshot-11.png)



> Now get your desired product and scrape the SKU's.
- Type the command ```?pds``` Followed by a URL or PID and it will scrape the SKU's and stock numbers.
- If Successful the bot will return all of the SKU's and stock like so.


![Scaper](https://i.ibb.co/gwJS8m0/Screenshot-2.png)



> Finally issue the ATC Command.
- Type the command ```?atc``` Followed by both the PID and the SKU desired with a **SPACE** in between the two.
- The bot will attempt to ATC and return the outcome and any errors.
- Should the bot successfully ATC it will return the basket details as followed.


![ATC](https://i.ibb.co/LYWsKng/Screenshot-3.png)

> Common Issues:
- If the bot returns a **500** error code it may be an issue with the PID/SKU requested, ensure it is correct or try another product.
- If the cookies become banned it will return an error 200 message with the response as:
- ```{"messages":{"notification":{"title":"We have encountered a problem","text":"Please Contact Us quoting 0.cf921602","type":"error","interval":3000}}}```
- If this is the case, the cookies will be banned along with the IP that generated them, use a VPN and gather new cookies. *(Most VPN's Work)*
