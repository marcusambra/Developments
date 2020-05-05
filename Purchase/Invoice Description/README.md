PURCHASE INVOICE DESCRIPTION
============================

Customer logged a request with Purchase Invoices “description” which they want to keep the same description from the Purchase Line once posted in the GL.

Currently the standard NAV creates GL entries “description” as per below:

![GL Entries](https://github.com/marcusambra/Images/blob/master/Purchase/Invoice%20Description/1-Image.png)

The customer wants to keep the same description from the purchase line as per the example below.
The Bal. Account will hold the standard description.

![GL Entries](https://github.com/marcusambra/Images/blob/master/Purchase/Invoice%20Description/2-Image.png)

Technical Details
------------------

Table: 49 – Invoice Post. Buffer
We have added a new field called “Posting Description”

![GL Entries](https://github.com/marcusambra/Images/blob/master/Purchase/Invoice%20Description/3-Image.png)

Table: 49 – Invoice Post. Buffer

Keys: Posting Description
The new key is needed to allow more then 2 lines with the same GL Account.

![GL Entries](https://github.com/marcusambra/Images/blob/master/Purchase/Invoice%20Description/4-Image.png)

Table: 49 - Invoice Post. Buffer
Trigger: PreparePurchase

We have added the folowing code:

![GL Entries](https://github.com/marcusambra/Images/blob/master/Purchase/Invoice%20Description/5-Image.png)

Codeunit: 90 – Purch.-Post
Function: SetupGenJnlLine

![GL Entries](https://github.com/marcusambra/Images/blob/master/Purchase/Invoice%20Description/6-Image.png)

object changes
--------------

![GL Entries](https://github.com/marcusambra/Images/blob/master/Purchase/Invoice%20Description/7-Image.png)

