### 线性代数的一些基础算法的python实现
`
用python实现了常用的线性代数的基础算法.用python2.7跑例子可以通过。不过很多细节没有考虑。
主要用来学习线性代数的一些算法原理

1. 方阵求逆
    采用类似LU分解的方法求矩阵的逆。
    inv.py

2. LU
    高斯消元法求解LU。  
    lu.py

3. 求方阵A的左零空间的基
   主要用来求解 Ax = 0的基础解。类似高斯消元法，求解给出了零空间的一组标准正交解
   null_space.py

4. 解线性方程组
   求解 Ax = b. 使用LU分解求解。 要求A是非奇异的。
   solve.py

5. QR分解
   使用  Gram-Schmidt正交化对矩阵进行QR分解
   qr.py

6.  QR分解求解矩阵的特征值和特征向量
    考虑了重根的情况。但没有考虑虚根等等
    eig_by_qr.py

7. 幂法、逆幂法求解最大、最小特征值 
    eig_by_pow_inverse.py

8. 对角化
   对矩阵A先求特征值和向量，然后进行对角化
    diagonalization.py

9. SVD实现
    先求A.T * A的特征向量，然后进行SVD分解
    svd.py

10. 求伪逆 
    实现了两个算法。 QR分解和SVD求伪逆
    pinv.py

11. 最小二乘法
    使用正规方程、QR分解、SVD分解、多项式拟合求解最小二乘
    SVD分解直接用的SVD求伪逆函数
    lstsq.py
