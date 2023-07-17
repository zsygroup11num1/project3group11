# project3group11
攻击步骤
1.随机生成一个消息(secret)，用SM3函数算出hash值(hash1)

2.生成一个附加消息(m')。首先用hash1推算出这一次加密结束后8个向量的值，再以它们作为初始向量，去加密m’，得到另一个hash值(hash2)

3.计算secret + padding + m'的hash值(hash3)，如果攻击成功，hash2应该和hash3相等

运行结果：![image](https://github.com/zsygroup11num1/project3group11/assets/129477117/27dee5e3-655b-4117-a8e7-dac39319ee5a)
