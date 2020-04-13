# Playing-with-digits
Playing with digits


import math
def dig_pow(n, p):
    n = str(n)
    count = 0
    for x in n:
        count = count + int(x) ** p
        p = p + 1
    count = count / int(n)
#     print(type(count))
    return count if math.floor(count) == count else -1
