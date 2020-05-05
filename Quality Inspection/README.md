QUALITY INSPECTION
==================

Setup
-----

1.  PURCHASE & PAYABLES SETUP

Define the “No. Series” for “Quality Inspection Order” and “Posted
Quality Inspection”

![Purchase Setup](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/Purchase_Setup_1.png)

2.  LOCATION

In the location card you can define the bin code for the Quality Inspection. This bin is normally defined as Quarantine or QA which you can segregate the item in your warehouse. 

The system will create a positive adjustment to the Bin Code informed in the field below

![Location](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/Location_card_2.png)

3.  ITEM CARD

Here you can define if the item should be inspected when a “purchase receipt” or Prod. Order Output” is posted.

![Item](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/Item_Card_3.png)

4.  VENDOR CARD

In the vendor Card you can define if all items from a specific vendor must be inspected once the purchase receipt is posted.

![Vendor](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/Vendor_Card_4.png)

PROCESS
-----

5.  PRUCHASE ORDER

There is a Boolean field in the “Purchase Line” called “Quality Inspection” which is automatically set as True if the item or Vendor has been set to true.

You can also mark this field manually if you want to create a Quality Inspection for an item which hasn’t been previously defined to be inspected.

![Purchase_order](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/purchase_order_5.png)

