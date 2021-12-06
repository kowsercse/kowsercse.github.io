---
title: Start Swagger Editor Locally
author: Kowser
date: 2021-12-05 03:43:00 -0800
categories: [Swagger, Tutorial]
tags: [swagger, tutorial]
---

[Swagger] offers

* [Swagger Editor]
* [Swagger UI]

## Swagger Editor

Run following script to start [Swagger Editor] locally. Download code from [Github][Swagger Github]

```console
git clone https://github.com/swagger-api/swagger-editor.git
cd swagger-editor
python3 -m http.server
```

Access the swagger editor at: <http://localhost:8000/>

## Swagger UI

Run following script to start [Swagger UI] locally. Download code from [Github][Swagger Github]

```console
git clone https://github.com/swagger-api/swagger-ui.git
cd swagger-ui/dist
python3 -m http.server
```

Access the swagger editor at: <http://localhost:8000/>

## References

* [Swagger]
* [Swagger Github]
* [Swagger Editor]
* [Swagger UI]

[Swagger]: <https://swagger.io/>
[Swagger Github]: <https://github.com/swagger-api/swagger-editor/>
[Swagger Editor]: <https://editor.swagger.io/>
[Swagger UI]: <https://petstore.swagger.io/>
