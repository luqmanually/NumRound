# NumRound

A function that formats a given number for text usage. It takes a single argument, num, which is the number to be formatted. The function returns a formatted string representing the number.

The function first takes the absolute value of the input number, then checks the magnitude of the number to determine the appropriate metric prefix to use. The metric prefixes used are:

- k (thousand)
- m (million)
- b (billion)
- t (trillion)

If the number is less than 1000, no metric prefix is used.

Once the metric prefix has been determined, the function formats the number to two decimal places if it is greater than 10, or three decimal places if it is less than 10.

Finally, the function adds the appropriate metric prefix to the formatted number and returns the result.

As an example, the following code would format the number 123456789 as "123.46m":

```js
const formattedNumber = numRound(123456789);
console.log(formattedNumber); // Output: "123.46m"
```
