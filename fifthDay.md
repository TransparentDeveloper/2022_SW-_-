5일차 실습예제 및 예시답안
-------------

### 1. 다음과 같은 파이썬 프로그램을 실행할 적에, 다음 밑줄 안에 들어갈 알맞은 결과는 무엇인가? 미리 예측해본 후 실행 시켜보고 그 결과를 적으시오.
'''
  
\>>> spell = ['s','w','e','e','t']  
\>>> spell   
(1) __________  
  
\>>> spell[3] = 'a'  
\>>> spell    
(2) __________  
  
\>>> spell[4] = 'r'  
\>>> spell   
(3) __________    
      
'''

```
#-----<예시 답안>------  

# 1) ['s','w','e','e','t']
# 2) ['s','w','e','a','t']
# 3) ['s','w','e','e','r']
  
 ```
 #

### 2. 다음과 같은 list1, list2 가 있을 경우 list1 과 list2 의 각 원소의 곱셈을 다음과 같이 출력하시오.
'''

list1 = [3,5,7]  
list2 =[2,3,4,5,6]  
  
--실행결과--   
    3 * 2 = 6  
    3 * 3 = 9  
    3 * 4 = 12  
    3 * 5 = 15  
    3 * 6 = 18  
    5 * 2 = 10  
    
'''

 ```
#-----<예시 답안>------

list1 = [3,5,7]  
list2 =[2,3,4,5,6] 


for i in range(len(list1)):
    for j in range(len(list2)):
        print("%d * %d = %d"%(list1[i],list2[j],list1[i]*list2[j]))
    
 ```
 #
 
 
### 3. a = [2,3,4,5,6]이 있을 경우, for-in문과 pop() 메소드를 사용하여 구현하시오.
### (힌트: 리스트의 원소를 하나하나 순회하면서 pop() 메소드를 호출하시오.)
'''
  
--실행결과--  
    a = [2,3,4,5,6]  
    rev_a = [6,5,4,3,2]  
      
'''

```  
#-----<예시 답안>------

def max2(m,n):
    if m>n:
        return m
    else :
        return n

def min2(m,n):
    if m>n:
        return n
    else :
        return m

print('100과 200중 큰 수는: ', max2(100,200))
print('100과 200중 작은 수는: ', min2(100,200))
  ```
 #   
 

### 4. 다음은 리스트를 이용한 프로그램이다. 빈 칸에 들어갈 알맞은 내용을 적으시오.
'''  
  
\>>> list1 = [2,3,4,1,32]  
   
\>>> list1.remove(32)  
\>>> list1  
1)_________  
  
\>>>list1.sort()  
\>>>list1  
2)_________   
     
'''  
  ```
#-----<예시 답안>------

# 1) [2,3,4,1]

# 2) [1,2,3,4,32]
    
  ```
 #     
 

### 5. n_list라는 리스트에 [10,20,30,50,60]과 같은 5개의 원소가 있다. n_list의 5개 원소의 합을 구하는 프로그램을 작성하여라.
'''  
   
-- 실행결과--  
    리스트의 원소들: [10,20,30,50,60]  
    리스트의 원소들의 합: 170  
  
'''  

  ```
#-----<예시 답안>------
  
n_list=[10,20,30,50,60]
sum = 0

for i in range(len(n_list)):
    sum += n_list[i]

print("리스트의 원소들의 합: %d" %(sum))
```
 #  
 

### 6. 임의의 정수값을 가진 리스트 n_list에서 가장 큰 값을 구하는 프로그램을 내장 함수를 사용하지 말고 구현하여라.
'''  
    
-- 실행결과--  
    리스트의 원소들 : [10,20,30,50,60]  
    리스트의 원소들 중 최댓값 : 60         
    
'''  
  ```
#-----<예시 답안>------
  
n_list = [10,20,30,50,60] 
max = n_list[0]

for i in range(1,len(n_list),1):
    if(max<n_list[i]):
        max = n_list[i]

print(max)
  ```
 # 
    
 

### 7. 다음 파이썬 프로그램의 수행결과를 예상하여 적으시오.
'''  
      
\>>> spell = ['h','a','p','p','y','b','i','r','t','h','d','a','y']  
  
\>>> spell[1:5]  
(1)_____________  
\>>> spell[:]  
(2)_____________  
\>>> spell[:5]  
(3)_____________  
\>>> spell[6:]  
(4)_____________  
\>>> spell[:2] + spell[9:]  
(5)_____________  

    
'''  
 ```
 

#-----<예시 답안>------

# (1) ['a','p','p','y']
# (2) ['h','a','p','p','y','b','i','r','t','h','d','a','y']
# (3) ['h','a','p','p','y']
# (4) ['i','r','t','h','d','a','y']
# (5) ['h','a','h','d','a','y']
 ```
 #
  
  
### 8. 동윤이가 새로 문을 열고 운영하는 커피 가게는 Americano, Ice Americano, Cappuccino, Caffe Latte, Espresso 의 5가지 메뉴가 있으며, 각 메뉴의 가격은 각각 3000원, 3500원, 4000원, 4500원, 3600원이다. 이 목록을 menu라는 딕셔너리로 작성하여라.
  
### 1) 이 menu의 내용을 for key in menu: 구문을 사용하여 다음과 같이 출력하여라.  

'''
  
-- 실행결과 --    
     
     Americano            가격: 3,000원  
     Ice Americano        가격: 3,500원  
     Cappuccino           가격: 4,000원  
     Caffe Latte          가격: 4,500원  
     Espresso             가격: 3,600원   

 '''

```
#-----<예시 답안>------
  
print("1)")
menu = {'Americano' : 5000 ,'Ice Americano' : 3500, 'Cappuccino' : 4000, 'Caffe Latte' : 4500 , 'Espresso' : 3600  }

for i in sorted(menu.keys()):
    price = str(menu[i])
    price = price[0] + "," + price[1:] + "원"
    print("%s\t가격: %s" %(i,price))
    
        
 ```


### 2) 사용자로부터 다음과 같은 주문을 받은 후 주문한 내용이 메뉴에 있는지 구하는 프로그램을 작성하여라(힌트: in 연산자를 사용할 것).  
  
 '''
 
-- 실행결과 --    
     
     Americano            가격: 3,000원  
     Ice Americano        가격: 3,500원  
     Cappuccino           가격: 4,000원  
     Caffe Latte          가격: 4,500원  
     Espresso             가격: 3,600원  
      
    위의 메뉴 중 하나를 선택하세요 : Espresso   
    Espresso 는 3,600원 입니다. 결제 부탁합니다.  

-- 실행결과 --  
     
     Americano            가격: 3,000원  
     Ice Americano        가격: 3,500원  
     Cappuccino           가격: 4,000원  
     Caffe Latte          가격: 4,500원  
     Espresso             가격: 3,600원  
  
    위의 메뉴 중 하나를 선택하세요 : Fan Cake     
    미안합니다. Fan Cake는 메뉴에 없습니다.  
'''  

 ```
 
#-----<예시 답안>------
  
menu = {'Americano' : 5000 ,'Ice Americano' : 3500, 'Cappuccino' : 4000, 'Caffe Latte' : 4500 , 'Espresso' : 3600  }

for i in sorted(menu.keys()):
    price = str(menu[i])
    price = price[0] + "," + price[1:] + "원"
    print("%s\t가격: %s" %(i,price))

want = str(input("위의 메뉴 중 하나를 선택하세요 : "))
is_check = False

for i in sorted(menu.keys()):
    if(i == want):
        is_check =True
        break
    else:
        is_check = False

if(is_check == True):
    price = str(menu[want])
    price = price[0] + "," + price[1:] + "원"
    print("%s 는 %s 입니다. 결제 부탁합니다." %(want, price))
else:
    print("미안합니다. %s는 메뉴에 없습니다." %(want))
    
 ```
 
 #
