---
title: "EInitializeNewDomainFlags 열거형"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: EInitializeNewDomainFlags
api_location: mscoree.dll
api_type: COM
f1_keywords: EInitializeNewDomainFlags
helpviewer_keywords: EInitializeNewDomainFlags enumeration [.NET Framework hosting]
ms.assetid: 3a120ab2-f5ef-4c9b-8595-d3ed7247c342
caps.latest.revision: "6"
author: rpetrusha
ms.author: ronpet
manager: wpickett
ms.openlocfilehash: bee1c5086502a9675e8149e7d6c9bc72f573815c
ms.sourcegitcommit: 4f3fef493080a43e70e951223894768d36ce430a
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/21/2017
---
# <a name="einitializenewdomainflags-enumeration"></a><span data-ttu-id="4e54f-102">EInitializeNewDomainFlags 열거형</span><span class="sxs-lookup"><span data-stu-id="4e54f-102">EInitializeNewDomainFlags Enumeration</span></span>
<span data-ttu-id="4e54f-103">런타임에 응용 프로그램 도메인의 초기화에 대 한 정보를 제공 하기 위해 호스트를 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4e54f-103">Enables the host to provide the runtime with information about the initialization of an application domain.</span></span>  
  
## <a name="syntax"></a><span data-ttu-id="4e54f-104">구문</span><span class="sxs-lookup"><span data-stu-id="4e54f-104">Syntax</span></span>  
  
```  
typedef enum {  
    eInitializeNewDomainFlags_None              = 0x0000,  
    eInitializeNewDomainFlags_NoSecurityChanges = 0x0002  
} EInitializeNewDomainFlags;  
```  
  
## <a name="members"></a><span data-ttu-id="4e54f-105">멤버</span><span class="sxs-lookup"><span data-stu-id="4e54f-105">Members</span></span>  
  
|<span data-ttu-id="4e54f-106">멤버</span><span class="sxs-lookup"><span data-stu-id="4e54f-106">Member</span></span>|<span data-ttu-id="4e54f-107">설명</span><span class="sxs-lookup"><span data-stu-id="4e54f-107">Description</span></span>|  
|------------|-----------------|  
|`eInitializeNewDomainFlags_None`|<span data-ttu-id="4e54f-108">플래그가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="4e54f-108">No flags.</span></span>|  
|`eInitializeNewDomainFlags_NoSecurityChanges`|<span data-ttu-id="4e54f-109">호스트에서 응용 프로그램 도메인의 보안 상태를 변경 하면 안 됩니다 공용 언어 런타임 (CLR) 알립니다는 <xref:System.AppDomainManager.InitializeNewDomain%2A> 메서드.</span><span class="sxs-lookup"><span data-stu-id="4e54f-109">Informs the common language runtime (CLR) that the host will not make changes to the security state of the application domain in the <xref:System.AppDomainManager.InitializeNewDomain%2A> method.</span></span>|  
  
## <a name="remarks"></a><span data-ttu-id="4e54f-110">설명</span><span class="sxs-lookup"><span data-stu-id="4e54f-110">Remarks</span></span>  
 <span data-ttu-id="4e54f-111">[iclrdomainmanager:: Setappdomainmanagertype](../../../../docs/framework/unmanaged-api/hosting/iclrdomainmanager-setappdomainmanagertype-method.md) 형식의 매개 변수를 사용 하는 메서드 `EInitializeNewDomainFlags`합니다.</span><span class="sxs-lookup"><span data-stu-id="4e54f-111">The [ICLRDomainManager::SetAppDomainManagerType](../../../../docs/framework/unmanaged-api/hosting/iclrdomainmanager-setappdomainmanagertype-method.md) method takes a parameter of type `EInitializeNewDomainFlags`.</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="4e54f-112">요구 사항</span><span class="sxs-lookup"><span data-stu-id="4e54f-112">Requirements</span></span>  
 <span data-ttu-id="4e54f-113">**플랫폼:** 참조 [시스템 요구 사항](../../../../docs/framework/get-started/system-requirements.md)합니다.</span><span class="sxs-lookup"><span data-stu-id="4e54f-113">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="4e54f-114">**헤더:** MSCorEE.h</span><span class="sxs-lookup"><span data-stu-id="4e54f-114">**Header:** MSCorEE.h</span></span>  
  
 <span data-ttu-id="4e54f-115">**라이브러리:** MSCorEE.dll</span><span class="sxs-lookup"><span data-stu-id="4e54f-115">**Library:** MSCorEE.dll</span></span>  
  
 <span data-ttu-id="4e54f-116">**.NET framework 버전:**[!INCLUDE[net_current_v40plus](../../../../includes/net-current-v40plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="4e54f-116">**.NET Framework Versions:** [!INCLUDE[net_current_v40plus](../../../../includes/net-current-v40plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="4e54f-117">참고 항목</span><span class="sxs-lookup"><span data-stu-id="4e54f-117">See Also</span></span>  
 [<span data-ttu-id="4e54f-118">호스팅 열거형</span><span class="sxs-lookup"><span data-stu-id="4e54f-118">Hosting Enumerations</span></span>](../../../../docs/framework/unmanaged-api/hosting/hosting-enumerations.md)  
 [<span data-ttu-id="4e54f-119">SetAppDomainManagerType 메서드</span><span class="sxs-lookup"><span data-stu-id="4e54f-119">SetAppDomainManagerType Method</span></span>](../../../../docs/framework/unmanaged-api/hosting/iclrdomainmanager-setappdomainmanagertype-method.md)