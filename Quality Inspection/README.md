QUALITY INSPECTION
==================

I have created a bespoke functionality in NAV to be used by the Quality team in order to inspect items received by suppliers and from production Order output.


Setup
-----

1.  PURCHASE & PAYABLES SETUP
-----------------------------

Define the “No. Series” for “Quality Inspection Order” and “Posted
Quality Inspection”

![Purchase Setup](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/Purchase_Setup_1.png)

2.  LOCATION
------------

In the location card you can define the bin code for the Quality Inspection. This bin is normally defined as Quarantine or QA which you can segregate the item in your warehouse. 

The system will create a positive adjustment to the Bin Code informed in the field below

![Location](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/Location_card_2.png)

3.  ITEM CARD
-------------

Here you can define if the item should be inspected when a “purchase receipt” or Prod. Order Output” is posted.

![Item](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/Item_Card_3.png)

4.  VENDOR CARD
---------------

In the vendor Card you can define if all items from a specific vendor must be inspected once the purchase receipt is posted.

![Vendor](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/Vendor_Card_4.png)

PROCESS
-----

5.  PURCHASE ORDER
------------------

There is a Boolean field in the “Purchase Line” called “Quality Inspection” which is automatically set as True if the item or Vendor has been set to true.

You can also mark this field manually if you want to create a Quality Inspection for an item which hasn’t been previously defined to be inspected.

![Purchase_order](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/purchase_order_5.png)

Once the “Purchase Receipt” is posted, then the Quality Inspection entry is created:

![Purchase_order](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/purchase_order_6.png)

If you navigate in the Warehouse Entry created from the Purchase Receipt, you will see the Positive Adjustment has been posted to the bin Code “QI” which was defined in the Location Card.

![Purchase_order](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/warehouse_posting_7.png)

6.  ITEM LEDGER ENTRY:
------------------

There is a FlowField which shows the Quality Inspection linked to the Item ledger Entry:

![Purchase_order](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/ILE_8.png)

In the item card you can also see how many quantities is/are in quality inspection:

![Item_Card](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/Item_9.png)

There is a validation which does not allow you to use the item, if the available item is on Quality Inspection.

![Validation](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/Error_10.png)


7.  Quality Inspection Order
-----
As can be seen below, the quality inspection was created, and it is open for inspection.

![QI](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/QI_11.png)

You can add comments in the line:

![QI](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/QI_12.png)

8.  Quality Check List:
-------------------

Here you can include all relevant information about the quality inspection process.

![QI](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/QI_13.png)

Once the Inspection Order was approved, then you can change the status to Closed

![QI](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/QI_14.png)

![QI](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/QI_15.png)

Once the status has been changed, the Quality Inspection has been transferred to Finished Quality Inspection List

![QI](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/QI_16.png)

![QI](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/QI_17.png)

9.  PRODUCTION ORDER
----------------

The same process applies to production orders, which the Quality Inspection will be created once the Output journal is posted

![QI](https://github.com/marcusambra/Developments/blob/master/Quality%20Inspection/Images/QI_18.png)

