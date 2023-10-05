<h1>Project Overview</h1>
There will be 3 tabs that user can switch to: <b>Debt, Add Debt, Payment</b>
<br><br>
Debt and Payment has a one to many relationship, meaning one debt can have
multiple payments linked to it.
<br><br>
<li>What if you fully paid one out of the four debt? How would the debt decrease? <br>
→ Debt would decrease proportional to the debt and payment ratio. for example, 1 dollar spent equates to 4 push up. if you do four push up, you would simply do the following: Debt = Debt - ((1/4) * 1/(total amount of payments)) * pushUpDone. Where (1/4) is the ratio that is set intially by the user. And total amount of payments depends on the user's payemnts for that debt. For example, 1 dollar spent requires 2 push up and 2 sit up as payment. Which means the total amount of payments required is <b>2</b>.
<br><br>
<li>Should we round down or round up for debt?
<br>
→ We'll allow debt to be in decimals, this will get rid of the need for rounding, and handling rounding error where all debt is paid, but debt is greater than 0 or less than 0.
<br><br>
<li>You can't pay past 0 in one form of payment, or should it be allowed?
<br>
→ Shouldn't allow payment past 0, if they are going to neglect all of the other payments, I think its better if they don't add it to their payment plan to begin with.
<br><br>
Debt and Payment can have overlapping payments. For example, 1 dollar debt requires 4 push ups. AND 10 calories for 3 push ups. In total, 1 dollar and 10 calories of debt means that user owes themselves 7 push ups.
<br><br>
<li>How to decrease debt, or which debt to decrease when there's two overlapping payments?
<br>
→ Pick the one with the smallest debt to payment ratio and decrease that debt. Users would probably like the method in which shows the most result, which in this case is the one with the smallest debt to payment ratio.
