# cho-han
#6/18 丁半プログラム　2個のサイコロの出る目の合計を予想して、結果が同じだったら勝ち
#100回やって何回かったかな
from vpython import*

import random

e=0
for i in range(100):
    
#予想
    a=[]
    for i in range(2):
        b=random.randint(1,6)
        a.append(b)
#     if (a[0]+a[1])%2==0:
#         print ("予想：丁",a)
#     else:
#         print("予想：半",a)


#実際のサイコロがどうなったか
    c=[]
    for i in range(2):
        d=random.randint(1,6)
        c.append(d)
#     if (c[0]+c[1])%2==0:
#         print("結果：丁",c)
#     else:
#         print("結果：半",c)

#勝敗の判定
# if (a[0]+a[1])%2==(c[0]+c[1])%2:
#     print("あなたの勝ち")
# else:
#     print("あなたの負け")

# n=int(input())
    if (a[0]+a[1])%2==(c[0]+c[1])%2:
        e=e+1
        f=100-e
print("100試合中:",e,"勝",f,"敗")
