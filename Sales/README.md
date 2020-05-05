AUTO ARCHIVE SALES DOCUMENT
==================

I have extended the standard auto archive functionality for sales order, which will archive the lateast version of the saler quote/order once the doucment is released.

This is useful for companies which want to track all modifications performed in the order before the document was released. 

SETUP
------

![Purchase Setup](https://github.com/marcusambra/Images/blob/master/Sales/Auto%20Archive/4_Image.png)


PROCESS
-------

Originally the document is only archived when the document is deleted (manually deleted or final posting).

![Sales Order](https://github.com/marcusambra/Images/blob/master/Sales/Auto%20Archive/1_Image.png)

Once the document is released, then the document will be automatically archived.

![Sales Order](https://github.com/marcusambra/Images/blob/master/Sales/Auto%20Archive/2_Image.png)


TECHINICAL DETAILS
-------------------

Table: 311-Sales & Receivables Setup: -	Created the new field below:

![Technical](https://github.com/marcusambra/Images/blob/master/Sales/Auto%20Archive/3_Image.png)

Page: 459-Sales & Receivables Setup

![Purchase Setup](https://github.com/marcusambra/Images/blob/master/Sales/Auto%20Archive/4_Image.png)


Codeunit: 414-Release Sales Document
![Purchase Setup](https://github.com/marcusambra/Images/blob/master/Sales/Auto%20Archive/5_Image.png)


OBJECT CHANGES
---------------
![Objects](https://github.com/marcusambra/Images/blob/master/Sales/Auto%20Archive/6_Image.png)



