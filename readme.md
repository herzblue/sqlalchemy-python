# 개요
## SQLAlchemy?
SQLAlchemy SQL Toolkit 및 Object Relational Mapper는 데이터베이스 및 Python 작업을 위한 포괄적인 도구 세트입니다.

SQLAlchemy는 SQL 표현식 언어 및 SQLAlchemy ORM을 포함하여 두 가지 주요 하위 패키지로 구성됩니다. SQLAlchemy SQL 표현식 언어는 SQL을 표현하기 위한 Python의 표현식 언어입니다. SQLAlchemy ORM은 Python 클래스를 데이터베이스 테이블로 매핑하는 방법을 제공합니다.

## SQLAlchemy Architecture
<!-- image -->
![SQLAlchemy](/asset/sqla_arch_small.png)

위에서 언급한 SQLAlchemy의 가장 중요한 두 가지 전면 부분은 ORM(Object Relational Mapper) 과 Core 입니다 .

- ORM은 Python 클래스를 데이터베이스 테이블로 매핑하는 방법을 제공합니다.
- Core는 SQL 표현식 언어를 사용하여 SQL을 표현하는 방법을 제공합니다.
- The SQL Expression Language는 SQL을 표현하기 위한 Python의 표현식 언어입니다.

## SQLAlchemy ORM

이 튜토리얼의 주요 섹션은 다음과 같습니다.

1. **연결 설정** - 엔진 - 모든 SQLAlchemy 애플리케이션은 Engine객체로 시작합니다. 만드는 방법은 다음과 같습니다.
2. **트랜잭션 및 DBAPI 작업**(Engine) - 및 관련 개체의 사용 API Connection 가Result여기에 표시됩니다. 이 콘텐츠는 핵심 중심이지만 ORM 사용자는 최소한 개체에 익숙해지기를 원할 것입니다 Result.
3. **데이터베이스 메타데이터 작업** - SQLAlchemy의 SQL 추상화와 ORM은 데이터베이스 스키마 구성을 Python 개체로 정의하는 시스템에 의존합니다. 이 섹션에서는 Core와 ORM 관점에서 이를 수행하는 방법을 소개합니다.
4. **데이터 작업** - 여기서는 데이터베이스에서 데이터를 생성, 선택, 업데이트 및 삭제하는 방법을 알아봅니다. 여기서 소위 CRUD 작업은 SQLAlchemy Core의 관점에서 제공되며, ORM 대응물에 대한 링크가 있습니다. SELECT 문 사용 에서 자세히 소개된 SELECT 작업은 Core와 ORM에 모두 동일하게 적용됩니다.
5. **ORM을 사용한 데이터 조작** - ORM의 지속성 프레임워크를 다룹니다. 기본적으로 ORM 중심의 삽입, 업데이트 및 삭제 방법과 트랜잭션 처리 방법입니다.
6. **ORM 관련 객체 작업** - 구문 의 개념을 소개 relationship()하고 더 깊은 문서에 대한 링크와 함께 구문의 사용 방법에 대한 간략한 개요를 제공합니다.