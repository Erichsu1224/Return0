# Atcoder Beginner 147 2019/12/8

## A & B
水到不能再水了  
兩題才花 3min

## C
**二進制枚舉**  
當 bit 為1時，表示那個人是誠實的

## D
這題直覺根據題目算式做會TLE  
做點變化變成 每一個bits (0的個數) * (1的個數) * 2^(第幾個bit) 相加  
  
但務必務必注意**每個動作都要mod**

## E
**背包問題**
用兩者差 枚舉所有可能  
dp[i][j][k+abs(a[i][j]-b[i][j])]  
dp[i][j][k-abs(a[i][j]-b[i][j])]

## F
**難題**  
把問題看成 Kx * Id (0 <= k <= n, (k-1) * k)/2 <= I <= (2 * n-k-1) * k)/2))  
並且 如果(K * x) % d 有相同值時，可以併成一組算(用Gready)  
時間複雜度可從 N^2 到 NlogN
