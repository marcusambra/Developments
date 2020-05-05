Production BOM - Approval Workflow
===================================

I have created an bespoke workflow to control the Bill of Material in the production module.

The status of the "Prod. BOM" can only be changed to certified if 
Technical Details
-----------------

1.Table: 99000771 – Production BOM Header
------------------------------------------
-	Created new field 50000 – Options: Open, Pending Approval, Released

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/1-Image.png)

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/2-Image.png)

2.Page 99000786 – Production BOM
---------------------------------

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/3-Image.png)
![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/4-Image.png)

3.Codeunit 1510: 49 – Notification Management
----------------------------------------------
GetDocumentTypeAndNumber

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/5-Image.png)

4.Codeunit 1520 – Workflow Event Handling
------------------------------------------

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/6-Image.png)

Function: RunWorkflowOnSendProdBOMforApprovalCode

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/7-Image.png)

Function: RunWorkflowOnSendProdBOMforApproval

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/8-Image.png)

Function: unWorkflowOnApproveApprovalRequestforProdBOMCode

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/9-Image.png)

Function: RunWorkflowOnApproveApprovalRequestforProdBOM

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/10-Image.png)

Function: RunWorkflowOnRejectApprovalRequestforProdBOMCode

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/11-Image.png)

Function: RunWorkflowOnRejectApprovalRequestforProdBOM

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/12-Image.png)

Function: RunWorkflowOnDelegateApprovalRequestforProdBOMCode

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/13-Image.png)

Function: RunWorkflowOnDelegateApprovalRequestforProdBOM

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/14-Image.png)

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/15-Image.png)

5.CODEUNIT: 1521
-------------------
Local - ReleaseDocument

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/16-Image.png)

Local - OpenDocument

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/17-Image.png)

6.CODEUNIT: 1535 – APPROVALS MGMT.
-----------------------------------
Function: SetStatusPendingApproval

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/18-Image.png)

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/19-Image.png)

Function: OnSendProdBOMforApproval

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/20-Image.png)

Function: IsProdBOMWorkflowEnabled

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/21-Image.png)

Function: CheckProdBOMWorkflowEnabled

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/22-Image.png)

Functiom: ShowProdBOMApprovalStatus

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/23-Image.png)

Function: IsProdBOMPendingApproval

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/24-Image.png)

Function: ShowProdBOMApprovalEntries

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/25-Image.png)

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/26-Image.png)

SETUP
------

Workflow – Table Relations
---------------------------

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/27-Image.png)

Workflow
--------

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/28-Image.png)


OBJECT CHANGES
---------------

![Tecnical](https://github.com/marcusambra/Images/blob/master/Workflow/BOMWorkflow/29-Image.png)



