# 021 문자열 인덱싱
### letters가 바인딩하는 문자열에서 첫번째와 세번째 문자를 출력하세요


```python
letters = 'python'
print(letters[0]+ ' ' + letters[2])
```

    p t
    


```python
# 022 문자열 슬라이싱
# 자동차 번호가 다음과 같을 때 뒤에 4자리만 출력하세요.
license_plate = "24가 2210"
print(license_plate[-4:])
```

    2210
    


```python
### 아래의 문자열에서 '홀' 만 출력하세요.
string = "홀짝홀짝홀짝"  
print (string[::2])
```

    홀홀홀
    


```python
#024 문자열 슬라이싱
#문자열을 거꾸로 뒤집어 출력하세요.
string = "PYTHON"
print(''.join(reversed(string)))
print(string[::-1])
```

    NOHTYP
    NOHTYP
    


```python
#025 문자열 치환
#아래의 전화번호에서 하이푼 ('-')을 제거하고 출력하세요.

phone_number = "010-1111-2222"
phone_number_replace = phone_number.replace("-"," ")
print(phone_number_replace)

#25번 문제의 전화번호를 아래와 같이 모두 붙여 출력하세요.
phone_number_replace = phone_number.replace("-","")
print(phone_number_replace)

```

    010 1111 2222
    01011112222
    


```python
#027 문자열 다루기
#url 에 저장된 웹 페이지 주소에서 도메인을 출력하세요.

url = "http://sharebook.kr"
url_idx = url.find(".")
print (url[url_idx+1:])

```

    kr
    


```python
#028 문자열은 immutable
#아래 코드의 실행 결과를 예상해보세요
```
lang = 'python'
lang[0] = 'P'
print(lang)

--> 문법 오류 문자열 일부 수정불가
```
```


```python
#29 replace 메서드
#아래 문자열에서 소문자 'a'를 대문자 'A'로 변경

string = 'abcdfe2a354a32a'
print (string.upper())

```

    ABCDFE2A354A32A
    

#030 replace 메서드
#아래 코드의 실행 결과를 예상해보세요.
```
>> string = 'abcd'
>> string.replace('b', 'B')
>> print(string)
>>수정 replace 메소드는 다른 저장소로 작업이 되므로 
```



```python
#031 문자열 합치기
#아래 코드의 실행 결과를 예상해보세요.

a = "3"
b = "4"
print(a + b)
# 문자이므로 병합 34
```

    34
    


```python
#032 문자열 곱하기
#아래 코드의 실행 결과를 예상해보세요.

print("Hi" * 3)
# HiHiHi
```

    HiHiHi
    


```python
##033 문자열 곱하기
#화면에 '-'를 80개 출력하세요.
print ("-" * 80)
```

    --------------------------------------------------------------------------------
    


```python
#034 문자열 곱하기
#변수에 다음과 같은 문자열이 바인딩되어 있습니다.

t1 = 'python'
t2 = 'java'
#변수에 문자열 더하기와 문자열 곱하기를 사용해서 아래와 같이 출력해보세요.
#실행 예:
#python java python java python java python java
print ((t1+' ' +t2+' ') * 4)
```

    python java python java python java python java 
    


```python
#035 문자열 출력
#변수에 다음과 같이 문자열과 정수가 바인딩되어 있을 때 % formatting을 사용해서 다음과 같이 출력해보세요.

name1 = "김민수" 
age1 = 10
name2 = "이철희"
age2 = 13
#이름: 김민수 나이: 10
#이름: 이철희 나이: 13
print("이름: %s 나이: %d" %(name1,age1))
print("이름: %s 나이: %d" %(name2,age2))

#036 문자열 출력
#문자열의 format( ) 메서드를 사용해서 035번 문제를 다시 풀어보세요.
print("036 문자열 출력")
print("이름: {0} 나이: {1}".format(name1,age1))
print("이름: {0} 나이: {1}".format(name2,age2))

#037 문자열 출력
#파이썬 3.6부터 지원하는 f-string을 사용해서 035번 문제를 다시 풀어보세요.
print("037 문자열 출력")
print(f"이름: {name1} 나이: {age1}")
print(f"이름: {name2} 나이: {age2}")

```

    이름: 김민수 나이: 10
    이름: 이철희 나이: 13
    036 문자열 출력
    이름: 김민수 나이: 10
    이름: 이철희 나이: 13
    037 문자열 출력
    이름: 김민수 나이: 10
    이름: 이철희 나이: 13
    


```python
#038 컴마 제거하기
#삼성전자의 상장주식수가 다음과 같습니다. 컴마를 제거한 후 이를 정수 타입으로 변환해보세요.

상장주식수 = "5,969,782,550"
상장주식수_int =  int(상장주식수.translate({ord(','): None}) )
print (type(상장주식수_int))
print (상장주식수_int)
```

    <class 'int'>
    5969782550
    


```python
#039 문자열 슬라이싱
#다음과 같은 문자열에서 '2020/03'만 출력하세요.

분기 = "2020/03(E) (IFRS연결)"
date_idx =분기.index('(')
print(분기[:date_idx])
```

    2020/03
    


```python
#040 strip 메서드
#문자열의 좌우의 공백이 있을 때 이를 제거해보세요.

data = "   삼성전자    "
print (data.strip())
```

    삼성전자
    


```python
#041 upper 메서드
#다음과 같은 문자열이 있을 때 이를 대문자 BTC_KRW로 변경하세요.

ticker = "btc_krw"
print(ticker.upper())

#042 lower 메서드
#다음과 같은 문자열이 있을 때 이를 소문자 btc_krw로 변경하세요.

tickerA = "BTC_KRW"
print(ticker.lower())

#043 capitalize 메서드
#문자열 'hello'가 있을 때 이를 'Hello'로 변경해보세요.
strC = "hello"
print(strC.capitalize())

#044 endswith 메서드
#파일 이름이 문자열로 저장되어 있을 때 endswith 메서드를 사용해서 파일 이름이 'xlsx'로 끝나는지 확인해보세요.

file_name = "보고서.xlsx"

file_name_chk = file_name.endswith('xlsx')

print(file_name_chk)

#045 endswith 메서드
#파일 이름이 문자열로 저장되어 있을 때 endswith 메서드를 사용해서 파일 이름이 'xlsx' 또는 'xls'로 끝나는지 확인해보세요.

file_name = "보고서.xlsx"
file_name_chk = file_name.endswith('xlsx') | file_name.endswith('xls')

print(file_name_chk)

#046 startswith 메서드
#파일 이름이 문자열로 저장되어 있을 때 startswith 메서드를 사용해서 파일 이름이 '2020'로 시작하는지 확인해보세요.

file_name = "2020_보고서.xlsx"
file_name_strswth = file_name.startswith('2020') 

print(file_name_strswth)

#047 split 메서드
#다음과 같은 문자열이 있을 때 공백을 기준으로 문자열을 나눠보세요.

a = "hello world"
print(a.split())

#048 split 메서드
#다음과 같이 문자열이 있을 때 btc와 krw로 나눠보세요.

ticker = "btc_krw"
print(ticker.split('_'))

#049 split 메서드
#다음과 같이 날짜를 표현하는 문자열이 있을 때 연도, 월, 일로 나눠보세요.

date = "2020-05-01"
date_l = date.split('-')
print(date_l)
print(type(date_l))

#050 rstrip 메서드
#문자열의 오른쪽에 공백이 있을 때 이를 제거해보세요.

data = "039490     "
print(data.rstrip())

```

    BTC_KRW
    btc_krw
    Hello
    True
    True
    True
    ['hello', 'world']
    ['btc', 'krw']
    ['2020', '05', '01']
    <class 'list'>
    039490
    


```python

```


```python

```


```python

```


```python

```


```python

정답확인
정답확인

```
