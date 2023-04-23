---
{"dg-publish":true,"title":"Bitcoin and Cryptocurrency Technologies","tags":["Crypto"],"permalink":"/Open-Courses/Bitcoin and Cryptocurrency Technologies/","dgPassFrontmatter":true,"created":"2023-04-22T21:47:34.179+08:00","updated":"2023-04-23T13:49:11.282+08:00"}
---

Course website: https://www.coursera.org/learn/cryptocurrency 
Text book(a complement to this course): https://bitcoinbook.cs.princeton.edu/ 
- pdf: https://d28rh4a8wq0iu5.cloudfront.net/bitcointech/readings/princeton_bitcoin_book.pdf


# Introduction to Crypto and Cryptocurrencies

## Cryptographic Hash Functions

Hash Function: 
- takes any strings as input
- fixd-size output (we'll use 256bits)
- efficiently computable
![img](https://www.thesslstore.com/blog/wp-content/uploads/2018/12/Hashing-Example.png)

Security properties:
- collision-free
	- Nobody can find x ang y such that x != y and H(x)=H(y), but collision do exists.
- hiding
	- Give H(x), it is infeasiable to find x.
- puzzle-friendly
	- For every possible output value y, if k is chosen from a distribution with high min-entropy, then it is infeasible to find x such that H(k | x)=y.
	- 就是说看x不知道H（x）是什么？这个无法从输入数据，判断到底输出是什么样子。就是说，知道输入的信息，无法一眼看出来输出的hash值是什么，谜题友好性值得就是这一点：你无法通过控制输入值x来获得想要的输出值H（x）。

SHA-256 hash function
	https://sha256algorithm.com/


## Hash Pointers and Data Structures
