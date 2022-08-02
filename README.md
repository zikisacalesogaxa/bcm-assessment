# BCM Assessment

Software to calculate the minimum number of coins required to return change to a user of Acme Vending machines.

For example, the vending machine uses the following coins denominations: 1,2,5 and 10 cents. If a user requires change of 43 cents what is the minimum number of coins required?

It would be 4 – 10 cents, 1 – 2 cents and 1 – 1 cent.

The coin denominations must be supplied as a parameter. This is so the algorithm is not specific to one country’s currency since Acme supplies vending machines to various countries around the world.

Please use the following country’s coin denominations to solve the problem:
- British Pound 1,2,5,10,20,50
- US Dollar 1,5,10,25

The problem assumes an infinite number of coins of each denomination.
You are to return an array populated with each coin’s denomination to be given as change.

### Example:

```javascript
var coinDenominations = [1,5,10,25]; // coin denominations – US Dollar
var machine = new VendingMachine(coinDenominations);
var purchaseAmount = 1.35; // amount the item cost
var tenderAmount = 2.00; // amount the user input for the purchase
var change = machine.CalculateChange(purchaseAmount, tenderAmount); // expect 65 cents
// The expected result would be an array that looks like
// change[0] = 25
// change[1] = 25
// change[2] = 10
// change[3] = 5
