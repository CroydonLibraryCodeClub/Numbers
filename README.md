# Numbers

## Converting from denary (decimal) to binary

Here is an easy algorithm to convert from decimal to binary, building your binary number from right to left:
1. if your decimal is odd, take 1 or if even, take 0 and put it on the left of your binary number
2. halve your decimal and, if you have anything left, go back to step 1.

### Example

Convert 57 (decimal) to binary

| take 1 if odd, 0 if even | insert on the left | halve what's left |
| - | -: | - |
| 57-**1** = 56 | **1** | 56/2 = 28 |
| 28-**0** = 28 | **0**1 | 28/2 = 14 |
| 14-**0** = 14 | **0**01 | 14/2 = 7 |
| 7-**1** = 6 | **1**001 | 6/2 = 3 |
| 3-**1** = 2 |  **1**1001 | 2/2 = 1 |
| 1-**1** = 0 | **1**11001 | | 

57 in decimal is 111001 in binary.

## Converting from binary to decimal

You can also use this algorithm backwards to convert from binary to decimal. This time you will be taking digits from your binary number from left to right:
1. take your leftmost binary digit and add it to your decimal
2. if you have any binary digits remaining, double your decimal and go back to step 1.

### Example

Convert 100011 (binary) to decimal

| remove from the left | decimal | double it |
| -: | - | - |
| **1**00011 | 0+**1** = 1 | 1\*2 = 2 |
| **0**0011 | 2+**0** = 2 | 2\*2 = 4 |
| **0**011 | 4+**0** = 4 | 4\*2 = 8 |
| **0**11 | 8+**0** = 8 | 8\*2 = 16 |
| **1**1 | 16+**1** = 17 | 17\*2 = 34 |
| **1** | 34+**1** = 35 |  |

100011 in binary is 35 in decimal.
