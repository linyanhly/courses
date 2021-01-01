
# solution

## lecture1

#### problem1-1. Asymptotic Practice

![image-20201203091635237](C:\Users\yan\AppData\Roaming\Typora\typora-user-images\image-20201203091635237.png)

**answer：f1(n) < f2(n) < f4(n) < f3(n)**


f1(n) 和 f2(n)之间的判断有一定的难度，但是对于f3(n)和f4(n)就可以通过二次方以及指数增加可以清楚地得知f4(n) < f3(n) and f4(n) > f2(n)，因此在这里f1(n)和f2(n)之间的判断即为此题的重点

 **logn∈O(nc) for any c>0 means:**

>For every c>0, there exists n0 ≥ 0 and k ≥ 0 such that logn ≤ k⋅n^c for all n ≥ n0.

因此：f1n)=n^0.999999*logn=O(n^0.999999\*n^0.000001)=O(n)=O(f2(n))

可以得知f1(n) < f2(n)

---



![image-20201203091653547](C:\Users\yan\AppData\Roaming\Typora\typora-user-images\image-20201203091653547.png)

**answer：f1(n) < f4(n) < f3(n) < f2(n)**



f1(n)为constant，而f2(n)为指数级增长，f3(n)为二次型，f4(n)为3/2次型

---

![image-20201203091850973](C:\Users\yan\AppData\Roaming\Typora\typora-user-images\image-20201203091850973.png)

**answer ：f4(n) < f1(n) < f3(n) < f2(n)**

在这里通过log变换，可以清晰地看到4个式子的大小

但是标准答案可能只是对各个式子做了一定的等效变换($2^{log_2^n}$)，这两种方法都可行且原理近似，对f1(n)和f3(n)做了指数变换，最终得到结果

---



#### Problem1-2.Recurrence Relation Resolution

![image-20201203094100735](C:\Users\yan\AppData\Roaming\Typora\typora-user-images\image-20201203094100735.png)

**answer：theta(n)**



可以写出递归公式，可以看出后面的部分都是小于2theta(x+y)，而且大于theta(x+y)，因此得知了最终的结果

---

![image-20201203094521401](C:\Users\yan\AppData\Roaming\Typora\typora-user-images\image-20201203094521401.png)

**answer：theta(nlogn)**



写出递归公式后，很清楚地推导出了最终的结果



---

![image-20201203094841084](C:\Users\yan\AppData\Roaming\Typora\typora-user-images\image-20201203094841084.png)

**answer：theta(n)**



注意在这里是可以消除递归式中的常数的，因此重写递归多项式后和(a)中的递归多项式一致，因此结果也一致





---





### Peak-Finding 

![image-20201203100033891](C:\Users\yan\AppData\Roaming\Typora\typora-user-images\image-20201203100033891.png)

---

#### Problem1-3.Peak-Finding Correctness

![image-20201203095846807](C:\Users\yan\AppData\Roaming\Typora\typora-user-images\image-20201203095846807.png)

**answer **

(a). 1

(b). 1

(c). 0

(d). 1

---

#### Problem 1-4. Peak-Finding Efficiency

![image-20201204092202104](C:\Users\yan\AppData\Roaming\Typora\typora-user-images\image-20201204092202104.png)

**answer**

(a). 3

(b). 5

(c). 2

(d). 2——得出递归公式，即可知道这里的原理

----

![image-20201204095840763](C:\Users\yan\AppData\Roaming\Typora\typora-user-images\image-20201204095840763.png)

the most efficient correct algorithm is the algorithm4, and the modification is as follow:

(a) Every recursive either the rows or the columns is down, so when the finally that this algorithm must return the outcome.

(b) we would choose the bestseen values instead the value we see now, 

----

![image-20201204100518367](C:\Users\yan\AppData\Roaming\Typora\typora-user-images\image-20201204100518367.png)