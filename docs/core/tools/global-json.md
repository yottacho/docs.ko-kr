---
title: global.json 참조
description: .NET Core 도구 버전 설정을 허용하는 global.json 파일의 스키마를 참조하세요.
author: blackdwarf
ms.author: mairaw
ms.date: 04/05/2017
ms.openlocfilehash: 7479774c7b9cdda233cf32d791c16e7fc6d733a8
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/04/2018
ms.locfileid: "33209972"
---
# <a name="globaljson-reference"></a>global.json 참조

*global.json* 파일을 사용하면 `sdk` 속성을 통해 사용 중인 .NET Core 도구 버전을 선택할 수 있습니다.

.NET Core CLI 도구는 현재 작업 디렉터리(프로젝트 디렉터리와 다를 수 있음) 또는 해당 부모 디렉터리 중 하나에서 이 파일을 찾습니다.

## <a name="sdk"></a>sdk
형식: Object

SDK에 대한 정보를 지정합니다.

### <a name="version"></a>버전
형식: String

사용할 SDK의 버전입니다.

예:

```json
{
  "sdk": {
    "version": "1.0.0-preview2-003121"
  }
}
```
