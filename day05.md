```python
# unit 20 Fizz Buzz 문제
# 1~100 까지의 숫자를 출력하면서, 3의 배수에는 Fizz를, 5의 배수에는 Buzz를
# 3과 5의 공배수에는 FizzBuzz를 출력하여라.

# 단계 1 : 1부터 100까지의 숫자를 출력
for i in range(1,101) : # 1부터 100까지 100번 반복
     print(i, end=" ") #print(i) 였던것을 뒤에 공백을 출력하게 바꿈
        
```

    1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46 47 48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63 64 65 66 67 68 69 70 71 72 73 74 75 76 77 78 79 80 81 82 83 84 85 86 87 88 89 90 91 92 93 94 95 96 97 98 99 100 


```python
# 단계 2 : 1부터 100까지의 숫자를 출력
#          3의 배수는 숫자대신 Fizz를 출력하여라
for i in range(1, 101):  #1부터 100까지 100번 반복
    if i % 3 == 0:       # 3의 배수일 때
        print('Fizz', end=" ")     # Fizz 출력
    else:
        print(i,end=" ")        # 아무것도 해당되지 않을 때 숫자 출력
```

    1 2 Fizz 4 5 Fizz 7 8 Fizz 10 11 Fizz 13 14 Fizz 16 17 Fizz 19 20 Fizz 22 23 Fizz 25 26 Fizz 28 29 Fizz 31 32 Fizz 34 35 Fizz 37 38 Fizz 40 41 Fizz 43 44 Fizz 46 47 Fizz 49 50 Fizz 52 53 Fizz 55 56 Fizz 58 59 Fizz 61 62 Fizz 64 65 Fizz 67 68 Fizz 70 71 Fizz 73 74 Fizz 76 77 Fizz 79 80 Fizz 82 83 Fizz 85 86 Fizz 88 89 Fizz 91 92 Fizz 94 95 Fizz 97 98 Fizz 100 


```python
# 단계 3 : 1부터 100까지의 숫자를 출력
#          3의 배수는 숫자대신 Fizz를 출력
#          5의 배수는 숫자대신 Buzz를 출력

for i in range(1, 101):  #1부터 100까지 100번 반복
    if i % 3 == 0:       # 3의 배수일 때
        print('Fizz', end=" ")     # Fizz 출력
    elif i % 5 == 0:    # 5의 배수일 때
        print('Buzz',end=" ")    # Buzz 출력
    else:
        print(i,end=" ")        # 아무것도 해당되지 않을 때 숫자 출력
```

    1 2 Fizz 4 Buzz Fizz 7 8 Fizz Buzz 11 Fizz 13 14 Fizz 16 17 Fizz 19 Buzz Fizz 22 23 Fizz Buzz 26 Fizz 28 29 Fizz 31 32 Fizz 34 Buzz Fizz 37 38 Fizz Buzz 41 Fizz 43 44 Fizz 46 47 Fizz 49 Buzz Fizz 52 53 Fizz Buzz 56 Fizz 58 59 Fizz 61 62 Fizz 64 Buzz Fizz 67 68 Fizz Buzz 71 Fizz 73 74 Fizz 76 77 Fizz 79 Buzz Fizz 82 83 Fizz Buzz 86 Fizz 88 89 Fizz 91 92 Fizz 94 Buzz Fizz 97 98 Fizz Buzz 


```python
# 단계 4 : 1부터 100까지의 숫자를 출력
#          3의 배수는 숫자대신 Fizz를 출력
#          5의 배수는 숫자대신 Buzz를 출력
#          3과 5의 공배수는 숫자대신 FizzBuzz를 출력

for i in range(1, 101):  #1부터 100까지 100번 반복
#     if i % 3 == 0 and i % 5 == 0:       # 3과 5의 공배수이면
#             print('FizzBuzz', end=" ")     # FizzBuzz 출력
    if i % 15 == 0 :    # 15의 공배수 이라면
        print('FizzBuzz', end=" ") 
    elif i % 5 == 0:    # 5의 배수일 때
        print('Buzz',end=" ")    # Buzz 출력
    else:
        print(i,end=" ")        # 아무것도 해당되지 않을 때 숫자 출력
```

    1 2 3 4 Buzz 6 7 8 9 Buzz 11 12 13 14 FizzBuzz 16 17 18 19 Buzz 21 22 23 24 Buzz 26 27 28 29 FizzBuzz 31 32 33 34 Buzz 36 37 38 39 Buzz 41 42 43 44 FizzBuzz 46 47 48 49 Buzz 51 52 53 54 Buzz 56 57 58 59 FizzBuzz 61 62 63 64 Buzz 66 67 68 69 Buzz 71 72 73 74 FizzBuzz 76 77 78 79 Buzz 81 82 83 84 Buzz 86 87 88 89 FizzBuzz 91 92 93 94 Buzz 96 97 98 99 Buzz 


```python
print('Fizz' *4)

for i in range(1,101):
    print('Fizz' * (i % 3 ==0) or i,end=" ")
```

    FizzFizzFizzFizz
    1 2 Fizz 4 5 Fizz 7 8 Fizz 10 11 Fizz 13 14 Fizz 16 17 Fizz 19 20 Fizz 22 23 Fizz 25 26 Fizz 28 29 Fizz 31 32 Fizz 34 35 Fizz 37 38 Fizz 40 41 Fizz 43 44 Fizz 46 47 Fizz 49 50 Fizz 52 53 Fizz 55 56 Fizz 58 59 Fizz 61 62 Fizz 64 65 Fizz 67 68 Fizz 70 71 Fizz 73 74 Fizz 76 77 Fizz 79 80 Fizz 82 83 Fizz 85 86 Fizz 88 89 Fizz 91 92 Fizz 94 95 Fizz 97 98 Fizz 100 


```python
# 다른접근: 1부터 100까지의 숫자를 출력
#          3의 배수는 숫자대신 Fizz를 출력
#          5의 배수는 숫자대신 Buzz를 출력
#          3과 5의 공배수는 숫자대신 FizzBuzz를 출력

for i in range(1,101):
    print('Fizz인디언' * (i % 3 ==0) + 'Buzz족장' * (1 % 5 ==0) or i,end="꼬마 ") #문자열 곱셈과 덧셈을 이용하여 print 안에서 처리
```

    1꼬마 2꼬마 Fizz인디언꼬마 4꼬마 5꼬마 Fizz인디언꼬마 7꼬마 8꼬마 Fizz인디언꼬마 10꼬마 11꼬마 Fizz인디언꼬마 13꼬마 14꼬마 Fizz인디언꼬마 16꼬마 17꼬마 Fizz인디언꼬마 19꼬마 20꼬마 Fizz인디언꼬마 22꼬마 23꼬마 Fizz인디언꼬마 25꼬마 26꼬마 Fizz인디언꼬마 28꼬마 29꼬마 Fizz인디언꼬마 31꼬마 32꼬마 Fizz인디언꼬마 34꼬마 35꼬마 Fizz인디언꼬마 37꼬마 38꼬마 Fizz인디언꼬마 40꼬마 41꼬마 Fizz인디언꼬마 43꼬마 44꼬마 Fizz인디언꼬마 46꼬마 47꼬마 Fizz인디언꼬마 49꼬마 50꼬마 Fizz인디언꼬마 52꼬마 53꼬마 Fizz인디언꼬마 55꼬마 56꼬마 Fizz인디언꼬마 58꼬마 59꼬마 Fizz인디언꼬마 61꼬마 62꼬마 Fizz인디언꼬마 64꼬마 65꼬마 Fizz인디언꼬마 67꼬마 68꼬마 Fizz인디언꼬마 70꼬마 71꼬마 Fizz인디언꼬마 73꼬마 74꼬마 Fizz인디언꼬마 76꼬마 77꼬마 Fizz인디언꼬마 79꼬마 80꼬마 Fizz인디언꼬마 82꼬마 83꼬마 Fizz인디언꼬마 85꼬마 86꼬마 Fizz인디언꼬마 88꼬마 89꼬마 Fizz인디언꼬마 91꼬마 92꼬마 Fizz인디언꼬마 94꼬마 95꼬마 Fizz인디언꼬마 97꼬마 98꼬마 Fizz인디언꼬마 100꼬마 


```python

```
