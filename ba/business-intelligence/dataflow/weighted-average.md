# Weighted Average

## What is Weighted average?

Weighted average is a calculation that takes into account the varying degrees of importance of the numbers in a data set. In calculating a weighted average, each number in the data set is multiplied by a predetermined weight before the final calculation is made.

A weighted average can be more accurate than a simple average in which all numbers in a data set are assigned an identical weight.

### Weighted average formula

<figure><img src="broken-reference" alt=""><figcaption></figcaption></figure>

### Example

| **Goods**            | **Quantity (w)** | Assigned Weight () | **Total amount (Data Point Weighted Value)** | **Stock**   | **Exchange stock** |
| -------------------- | ---------------- | ------------------ | -------------------------------------------- | ----------- | ------------------ |
| Product a            | 10               | 2                  | 20                                           | Inventory A |                    |
| Product a            | 50               | 5                  | 250                                          | Inventory A |                    |
| Product a            | 40               | 3                  | 120                                          | Inventory A |                    |
| **TOTAL**            | **100**          | **10**             | **390**                                      |             |                    |
| **Weighted Average** |                  |                    | _**39**_                                     |             |                    |

## Weighted average node in Symper BI

Weighted average node has 5 configuration elements:

**Goods:** determine the object to be calculated

**Stock:** Separate the goods into groups of each stocks

**Exchange Stock:** In case of good have transaction forward and backward at the same time

**Quantity:** Determine number of good in each transaction

**Total amount**: Determine the weighted value of good

An use case that Weighted average node solve: [https://sites.google.com/site/tailieuhocngoaingutinhoc/tin-hoc/phan-mem-ke-toan/fast-accounting/fast-accounting-online/huong-dan-su-dung/ton-kho/tinh-gia-trung-binh](https://sites.google.com/site/tailieuhocngoaingutinhoc/tin-hoc/phan-mem-ke-toan/fast-accounting/fast-accounting-online/huong-dan-su-dung/ton-kho/tinh-gia-trung-binh)

## How the weighted average node (WAN) work?

In real world, the most complicated case will be All the transaction of each good have the exchange stock. That mean the weighted average of good depends on both forward transaction and backward transaction at the same time.

To solve the problem, the **WAN** has to solve the **set of equation.**

To narrow down the problem complication, Symper use the **Linear Algebra** to solve the set of equation.

The set of equation:

<figure><img src="broken-reference" alt=""><figcaption></figcaption></figure>

Using **Cramer's rule** to solve set of equation ([you can find more detail of cramer's rule here](https://en.wikipedia.org/wiki/Cramer's\_rule)).
