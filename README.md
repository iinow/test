---
title: 공통 공지 v0.1
language_tabs:
  - http: HTTP
language_clients:
  - http: ""
toc_footers: []
includes: []
search: true
highlight_theme: darkula
headingLevel: 2

---

<!-- Generator: Widdershins v4.0.1 -->

<h1 id="-">공통 공지 v0.1</h1>

> Scroll down for code samples, example requests and responses. Select a language for code samples from the tabs above or the mobile navigation menu.

공통 공지 API 문서 입니다.

Base URLs:

* <a href="http://localhost:8080">http://localhost:8080</a>

<h1 id="--foo-controller">foo-controller</h1>

## foo2

<a id="opIdfoo2"></a>

> Code samples

```http
GET http://localhost:8080/test HTTP/1.1
Host: localhost:8080
Accept: */*

```

`GET /test`

yearMonth?

<h3 id="foo2-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|name|query|string|false|하하하하하 이름 |

> Example responses

> 200 Response

<h3 id="foo2-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|

<h3 id="foo2-responseschema">Response Schema</h3>

<aside class="success">
This operation does not require authentication
</aside>

## foo_1

<a id="opIdfoo_1"></a>

> Code samples

```http
GET http://localhost:8080/ HTTP/1.1
Host: localhost:8080
Accept: */*

```

`GET /`

하하

<h3 id="foo_1-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|name|query|string|false|하하하하하 이름 |

> Example responses

> default Response

<h3 id="foo_1-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|default|Default|default response|[ApiResponseRPerson](#schemaapiresponserperson)|

<aside class="success">
This operation does not require authentication
</aside>

<h1 id="--bar-controller">bar-controller</h1>

## bar

<a id="opIdbar"></a>

> Code samples

```http
GET http://localhost:8080/bar?size=10&page=0 HTTP/1.1
Host: localhost:8080
Accept: */*

```

`GET /bar`

<h3 id="bar-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|size|query|integer(int32)|true|사이즈|
|page|query|integer(int32)|true|페이지 번호|

> Example responses

> 200 Response

<h3 id="bar-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|

<h3 id="bar-responseschema">Response Schema</h3>

<aside class="success">
This operation does not require authentication
</aside>

# Schemas

<h2 id="tocS_ApiResponseRPerson">ApiResponseRPerson</h2>
<!-- backwards compatibility -->
<a id="schemaapiresponserperson"></a>
<a id="schema_ApiResponseRPerson"></a>
<a id="tocSapiresponserperson"></a>
<a id="tocsapiresponserperson"></a>

```json
{
  "success": true,
  "data": {
    "name": "하하호홓"
  }
}

```

공통 응답

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|success|boolean|false|none|none|
|data|[RPerson](#schemarperson)|false|none|none|

<h2 id="tocS_RPerson">RPerson</h2>
<!-- backwards compatibility -->
<a id="schemarperson"></a>
<a id="schema_RPerson"></a>
<a id="tocSrperson"></a>
<a id="tocsrperson"></a>

```json
{
  "name": "하하호홓"
}

```

유저 응답 값

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|name|string|true|none|none|

