# SQL-ProblemSolving

* [Programmers](https://github.com/yaezzin/SQL-Study/tree/main/Programmers/)
* [LeetCode](https://github.com/yaezzin/SQL-Study/tree/main/LeetCode)
* [Hackerrank]()

## Note

|Command|Description|
|-------|----------|
|```IFNULL(A, B)``` | A가 NULL일 경우 B를 출력|
|```A IS NULL```|컬럼 A가 NULL이라면 (WHERE절에 주로 사용)|
|```A IS NOT NULL```|컬럼 A가 NULL이 아니라면 (WHERE절에 주로 사용)|
|```DISTINCT```|중복된 데이터를 제거하고 데이터를 조회|
|```LIKE 'A%'```|A로 시작하는 문자 찾기|
|```LIKE '%A'```|A로 끝나는 문자 찾기|
|```LIKE '%A%'```|A를 포함하는 문자 찾기|
|```COUNT(A)```|A의 개수를 리턴|
|```AVG(A)```|A의 평균을 리턴|
|```SUM(A)```|A의 합을 리턴|
|```MAX(A)```|- A의 최대값을 리턴 </br> - DATETIME 컬럼을 넣을 경우 가장 최신 날짜를 리턴|
|```MIN(A)```|- A의 최솟값을 리턴 </br> - DATETIME 컬럼을 넣을 경우 가장 오래된 날짜를 리턴|
|```ROUND(N, M)``` |- 숫자 N을 소수점 M째 자리에서 반올림 </br> - 반올림할 위치에 아무것도 적지 않으면 첫째 자리에서 반올림을 하며, 1을 적을경우부터 둘째자리에서 반올림|
|```DATE_FORMAT(D, F)``` | - 날짜 D를 형식 F에 맞게 리턴 </br> - ex) **DATE_FORMAT(NOW(),'%Y-%m-%d')**|
|```YEAR(D)```|날짜 D의 '연도' 값을 리턴|
|```MONTH(D)```|날짜 D의 '월' 값을 리턴|
|```DAYOFMONTH(NOW()```|날짜 D의 '일' 값을 리턴|

## GROUP BY

> 같은 값을 가진 행을 그룹짓는 SQL 명령어

* GROUP BY는 COUNT(), MAX(), MIN(), SUM(), AVG() 등 집계 함수와 함께 사용
* DISTINCT처럼 그룹화하는 과정에서 중복이 제거되는 기능도 하나, 중복제거만을 위해서라면 DISTINCT를 사용하는 것이 좋음

## HAVING

> GROUP BY절에 의해 그룹핑한 행에 대해 원하는 조건에 부합하는 데이터만 보고자 할 때 사용
* WHERE절은 행들이 그룹핑되기 전 단일 행들을 필터링하는 데 사용 = WHERE 절이 GROUP BY 전에 적힘
* HAVING 절은 행들이 그룹핑된 후의 행들을 필터링하는 데 사용 = HAVING 절이 GROUP BY 후에 적힘
