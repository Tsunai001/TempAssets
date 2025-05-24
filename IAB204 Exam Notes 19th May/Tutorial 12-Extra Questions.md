1. Use Case Diagram
In an eCommerce application, a registered customer begins their journey by logging into their account. Having browsed through the catalogue, they've added a few desired items to their shopping cart. Now ready to complete the purchase, the customer navigates to the shopping cart page to review their selections. They carefully check the product details, quantities, and prices to ensure everything is in order.
Satisfied with the contents of the cart, the customer clicks the "Checkout" button. The system then prompts them to enter or confirm their shipping details. If the address is invalid or incomplete, the system immediately flags the issue and requests corrections. The customer updates the address and proceeds.
Next, the system asks the customer to choose a payment method. The customer selects their preferred option and enters the necessary payment details. If the payment fails due to incorrect information or insufficient funds, the system notifies the customer, who then either corrects the details or selects an alternative payment method.
Once the payment is successfully processed, the system confirms the transaction and generates an order. However, if any item in the cart is found to be out of stock at this stage, the system alerts the customer, offering alternatives or removing the unavailable item. The customer can then update the cart and retry the checkout process.
With everything in place, the system finalizes the order, sends a confirmation email to the customer, and updates the inventory and order history in real time. Throughout the process, the application ensures secure handling of payment information in compliance with PCI DSS standards and provides a responsive experience across both mobile and desktop devices.
In the end, the customer successfully places their order, confident in the seamless and secure transaction experience provided by the eCommerce platform.

Solution:
Use Case Title: Place Order
Primary Actor: Customer
Goal: To successfully place an order for one or more products.
Scope: Ecommerce Application
Level: User Goal
Preconditions:
* The customer is registered and logged into the system.
* The customer has added at least one item to the shopping cart.
Postconditions:
* The order is saved in the system.
* The customer receives an order confirmation.
* Inventory is updated accordingly.
Main Success Scenario:
1. Customer navigates to the shopping cart.
2. Customer reviews the items in the cart.
3. Customer clicks on the "Checkout" button.
4. System prompts the customer to enter or confirm shipping details.
5. Customer enters or confirms shipping information.
6. System prompts the customer to select a payment method.
7. Customer selects a payment method and enters payment details.
8. System processes the payment.
9. System confirms the payment and generates an order.
10. System sends an order confirmation email to the customer.
11. System updates the inventory and order history.
Extensions:
* 4a. Invalid Shipping Address:
* 4a1. System detects invalid or incomplete shipping address.
* 4a2. System prompts the customer to correct the address.
* 4a3. Customer corrects and resubmits the address.
* 7a. Payment Failure:
* 7a1. System fails to process the payment.
* 7a2. System notifies the customer of the failure.
* 7a3. Customer retries with a different payment method or corrects the payment details.
* 9a. Out of Stock:
* 9a1. System detects one or more items are out of stock.
* 9a2. System notifies the customer and suggests alternatives or removes the item.
* 9a3. Customer updates the cart and retries checkout.
Special Requirements:
* Secure handling of payment information (PCI DSS compliance).
* Real-time inventory updates.
* Responsive design for mobile and desktop users.

2. Decision Tree:
Intellicube System Pty is an Australian software development firm. The management is worried about its business growth and is interested in a new and innovative software solution to compete in the market. The management has the following options to make a final decision. 

Option 1. Embark into Robotic Process Automation (RPA) Market by developing its own AI-based RPA solution. OR 
Option 2. Act as an intermediary by collaborating with an existing RPA solution provider. OR
Option 3. Continue as-is without introducing either of the two options. 

This 1st option will cost $1,800,000 for setting up the required infrastructure and equipment. The marketing department estimates that the market will react favourably with a 60% probability and sales of the new RPA solution will hit $4,500,000. However, there is a 40% probability that the new RPA solution may not be appreciated by potential clients. In that case, estimated revenue will be $1,500,000. 

The 2nd option will cost $500,000 to get the required licences and partner status. The marketing department estimates a 70% probability of success and new services will bring $2,000,000 in revenue. In case of an unfavourable market response, the estimated revenue will be $400,000. 

3. Cost-Benefit Analysis
You are requested to help the management to prioritise their decision by providing an Expected Monetary Analysis using the Decision Tree technique. 
A small café is considering replacing one of its waitstaff with a 'robot'
- a device that will take orders, deliver food and interact with customers in an entertaining way. The cost of the robot is $225,000. From the salary savings and the extra customers the robot is expected to attract, it is estimated that the net inflows from the idea will be:

* Year 1: $95,000
* Year 2: $80,000
* Year 3: $60,000
* Year 4: $55,000
It is expected that novelty will lessen over time, and after four years the robot will be worthless and superseded with a newer model.

TASK 1: Using the formulas and examples from the lectures, perform a cost benefit analysis by calculating the payback period (PBP), the return on investment (ROI), the Net Present Value (NPV) and the Internal Rate of Return (IRR). Assume the desired rate of return is 12%.
TASK 2: On the basis of your cost-benefit analysis, would you recommend that the café proceed?
