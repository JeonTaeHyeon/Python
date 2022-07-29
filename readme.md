## 슬라이싱

```python
a="12345678"

print(a[0:4:2])
```
>실행결과 : 13

0에서 4까지 간격 2를 가지고 출력
```python
a="12345678"

print(a[::-1])
```
>실행결과 : 87654321

##  Formating
```python
a="i name is {name} i was born in {year}".format(name="Jeon",year=2000)
print(a)
```
>실행결과 : i name is Jeon i was born in 2000
##  문자열
#### 	- find, count
```python
a="my name is aaa"

print(a.count('a'))

print(a.find('y'))
```
>실행결과 : 
>4
1

count는 갯수를 세고 find는 index가 가장 해당 문자의 index를 출력한다.
#### join
```python
a="m".join("abcde")

print(a)
```
>실행결과 : ambmcmdme

문자열 사이에 끼워넣기

#### lower(소문자로 바꾸기), upper(대문자로 바꾸기), strip(양쪽 공백 지우기)
#### split
```python
a="one two three four"

print(a.split())
```
>실행결과 : ['one', 'two', 'three', 'four']

## list
```python
a= ["one","two",["three","four"]]

print(a)

print(a[2])

print(a[2][1])
```
>실행결과 : 
['one', 'two', ['three', 'four']]
['three', 'four']
four

append, recverse, index, sort, del, insert, remove, pop, count, extend

## tuple
리스트랑 다르게 고정된 것 
```python
a= (1,2,3,4)
print(a)
```
>실행결과 :  (1, 2, 3, 4)
## 딕셔너리

```python
a= {"name":"Joen"}

a["age"]=20
print(a)

del  a["age"]
print(a )
```
> 실행결과 : 
> {'name': 'Joen', 'age': 20}
{'name': 'Joen'}

key, value를 저장하는 자료형 key를 사용하여 del할 수 있음 key를 이용하여 value를 조회할 수 있음, key는 중복될 수 없다.


```python
a= {"name":"Joen"}

a["age"]=20

print(a.keys())

print(a.values())
```
> 실행결과 : 
> dict_keys(['name', 'age'])
dict_values(['Joen', 20])

key또는 value만 조회할 수도 있음.
## set
```phthon
a= set([1,2,3])

print(a)

b={1,2,3}

print(b)
```
> 실행결과 : 
> {1, 2, 3}
{1, 2, 3}

집합은 중복이 안됨 
#### 활용
``` python
li=[1,1,2,2,3,3,3,3]

print(li)

  

s=set(li)

print (s)
```
> 실행결과 : 
> [1, 1, 2, 2, 3, 3, 3, 3]
{1, 2, 3}

#### 교집합(intersaction) 합집합(union) 차집합(difference)
```python
s1={1,2,3,4,5,6}

s2={5,6,7,8,9}

  

print(s1&s2)

print(s1|s2)

print(s1-s2)
```
> 실행결과 :
{5, 6}
{1, 2, 3, 4, 5, 6, 7, 8, 9}
{1, 2, 3, 4}
####  add, update, remove
```python
s1={1,2,3,4,5,6}

s1.add(7)

print(s1)


s1.update([8,9])

print(s1)

s1.remove(1)
print(s1)
```
> 실행결과 : 
> {1, 2, 3, 4, 5, 6, 7}
{1, 2, 3, 4, 5, 6, 7, 8, 9}
{2, 3, 4, 5, 6, 7, 8, 9}


## 반복문
```python
#for 기본형

li =["one","two","three"]

  

for  i  in  li :

print(i)

  

li=[["one","two"],["three","four"]]

for  i  in  li:

print(i)
```
>  실행결과
> one
two
three
['one', 'two']
['three', 'four']

## 리스트 내포(list comprehension)
```python


```
>
