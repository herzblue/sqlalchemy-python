# 개요
* python SQLalchemy 동작원리 이해

<br>

# 요약
* proxy 패턴을 사용하여 database와 engine을 컨트롤
* 컨트롤을 위한 임시 캐시 공간을 session이라고 정의
> 비슷한 아키텍처를 가진 JPA에서는 Entinity Manager라고 부릅니다.
* session.commit()을 호출하기 전까지는 캐시에 저장된 데이터베이스를 사용

<br>

# 파일 설명
* [orm을 미사용](NOT_ORM.ipynb)
* [orm을 사용](ORM.ipynb)

<br>

# 참고자료 
* [1] 블로그 - https://leportella.com/sqlalchemy-tutorial/
* [2] 공식문서 - https://docs.sqlalchemy.org/en/14/orm/tutorial.html