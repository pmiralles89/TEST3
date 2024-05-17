# TEST3
# Steven's Tip Calculator
## What It Is
This is a simple tool to calculate tips when you're eating out. It helps you figure out how much tip to leave based on your bill.
## Why It's Made
The goal is to make tipping easy:
- If your bill is between $50 and $300, it calculates a 15% tip.
- For anything else, it calculates a 20% tip.
## How to Use It
Just enter your bill amount, and it'll tell you:
- Your bill
- The tip amount
- Your total (bill + tip)
## Try It Out
## Calculate the Tip

To determine the tip based on the bill amount:
```javascript
const tip = bill >= 50 && bill <= 300 ? bill * 0.15 : bill * 0.2;```

## Output Details

Displaying the calculation results:
```javascript
console.log(`The bill was $${bill}, the tip was $${tip}, and the total value $${bill + tip}`);```

## calcTip Function

Function to calculate the tip:
```javascript
function calcTip(bill) {
  return bill >= 50 && bill <= 300 ? bill * 0.15 : bill * 0.2;```
}

// Testing the function
const testTip = calcTip(100);

## Working with Arrays

Using arrays for bills, tips, and totals:
```javascript
const bills = [125, 555, 44];
const tips = bills.map(bill => calcTip(bill));
const totals = bills.map((bill, index) => bill + tips[index]);```
