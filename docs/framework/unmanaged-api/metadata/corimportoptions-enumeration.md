---
title: "CorImportOptions 열거형"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: CorImportOptions
api_location: mscoree.dll
api_type: COM
f1_keywords: CorImportOptions
helpviewer_keywords: CorImportOptions enumeration [.NET Framework metadata]
ms.assetid: 4e5d03cb-97c9-4ff4-8dbd-17d94ee374d3
topic_type: apiref
caps.latest.revision: "7"
author: mairaw
ms.author: mairaw
manager: wpickett
ms.openlocfilehash: 3e014443945574cff2733e5bc5d992691acc3fd9
ms.sourcegitcommit: bd1ef61f4bb794b25383d3d72e71041a5ced172e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/18/2017
---
# <a name="corimportoptions-enumeration"></a><span data-ttu-id="d7672-102">CorImportOptions 열거형</span><span class="sxs-lookup"><span data-stu-id="d7672-102">CorImportOptions Enumeration</span></span>
<span data-ttu-id="d7672-103">현재 범위를 벗어난 어셈블리를 가져오는 중의 동작을 제어하는 플래그 값을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="d7672-103">Contains flag values that control the behavior during importation of an assembly outside the current scope.</span></span>  
  
## <a name="syntax"></a><span data-ttu-id="d7672-104">구문</span><span class="sxs-lookup"><span data-stu-id="d7672-104">Syntax</span></span>  
  
```  
typedef enum CorImportOptions {  
  
    MDImportOptionDefault                = 0x00000000,  
    MDImportOptionAll                    = 0xFFFFFFFF,  
    MDImportOptionAllTypeDefs            = 0x00000001,  
    MDImportOptionAllMethodDefs          = 0x00000002,  
    MDImportOptionAllFieldDefs           = 0x00000004,  
    MDImportOptionAllProperties          = 0x00000008,  
    MDImportOptionAllEvents              = 0x00000010,  
    MDImportOptionAllCustomAttributes    = 0x00000020,  
    MDImportOptionAllExportedTypes       = 0x00000040  
  
} CorImportOptions;  
```  
  
## <a name="members"></a><span data-ttu-id="d7672-105">멤버</span><span class="sxs-lookup"><span data-stu-id="d7672-105">Members</span></span>  
  
|<span data-ttu-id="d7672-106">멤버</span><span class="sxs-lookup"><span data-stu-id="d7672-106">Member</span></span>|<span data-ttu-id="d7672-107">설명</span><span class="sxs-lookup"><span data-stu-id="d7672-107">Description</span></span>|  
|------------|-----------------|  
|`MDImportOptionDefault`|<span data-ttu-id="d7672-108">삭제 된 레코드는 건너 뜁니다 하는 기본 동작을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="d7672-108">Indicates the default behavior, which is to skip deleted records.</span></span>|  
|`MDImportOptionAll`|<span data-ttu-id="d7672-109">모든 메타 데이터를 열거 해야 함을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="d7672-109">Indicates that all metadata should be enumerated.</span></span>|  
|`MDImportOptionAllTypeDefs`|<span data-ttu-id="d7672-110">삭제 된 항목을 포함 하 여 모든 형식 정의 열거 해야 함을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="d7672-110">Indicates that all TypeDefs, including deleted ones, should be enumerated.</span></span>|  
|`MDImportOptionAllMethodDefs`|<span data-ttu-id="d7672-111">모든 MethodDefs, 삭제 된 항목을 포함 하 여 열거 해야 함을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="d7672-111">Indicates that all MethodDefs, including deleted ones, should be enumerated.</span></span>|  
|`MDImportOptionAllFieldDefs`|<span data-ttu-id="d7672-112">삭제 된 항목을 포함 하 여 모든 Fielddef 열거 해야 함을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="d7672-112">Indicates that all FieldDefs, including deleted ones, should be enumerated.</span></span>|  
|`MDImportOptionAllProperties`|<span data-ttu-id="d7672-113">모든 PropertyDefs, 삭제 된 항목을 포함 하 여 열거 해야 함을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="d7672-113">Indicates that all PropertyDefs, including deleted ones, should be enumerated.</span></span>|  
|`MDImportOptionAllEvents`|<span data-ttu-id="d7672-114">삭제 된 항목을 포함 하 여 모든 Eventdef 열거 해야 함을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="d7672-114">Indicates that all EventDefs, including deleted ones, should be enumerated.</span></span>|  
|`MDImportOptionAllCustomAttributes`|<span data-ttu-id="d7672-115">삭제 된 항목을 포함 하 여 모든 사용자 지정 특성을 열거 해야 함을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="d7672-115">Indicates that all custom attributes, including deleted ones, should be enumerated.</span></span>|  
|`MDImportOptionAllExportedTypes`|<span data-ttu-id="d7672-116">삭제 된 항목을 포함 하는 모든 내보낸된 형식을 열거 해야 함을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="d7672-116">Indicates that all exported types, including deleted ones, should be enumerated.</span></span>|  
  
## <a name="requirements"></a><span data-ttu-id="d7672-117">요구 사항</span><span class="sxs-lookup"><span data-stu-id="d7672-117">Requirements</span></span>  
 <span data-ttu-id="d7672-118">**플랫폼:** 참조 [시스템 요구 사항](../../../../docs/framework/get-started/system-requirements.md)합니다.</span><span class="sxs-lookup"><span data-stu-id="d7672-118">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="d7672-119">**헤더:** CorHdr.h</span><span class="sxs-lookup"><span data-stu-id="d7672-119">**Header:** CorHdr.h</span></span>  
  
 <span data-ttu-id="d7672-120">**.NET framework 버전:**[!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="d7672-120">**.NET Framework Versions:** [!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="d7672-121">참고 항목</span><span class="sxs-lookup"><span data-stu-id="d7672-121">See Also</span></span>  
 [<span data-ttu-id="d7672-122">메타 데이터 열거형</span><span class="sxs-lookup"><span data-stu-id="d7672-122">Metadata Enumerations</span></span>](../../../../docs/framework/unmanaged-api/metadata/metadata-enumerations.md)