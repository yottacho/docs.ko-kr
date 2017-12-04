---
title: "ICLRErrorReportingManager::EndCustomDump 메서드"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: ICLRErrorReportingManager.EndCustomDump
api_location: mscoree.dll
api_type: COM
f1_keywords: ICLRErrorReportingManager::EndCustomDump
helpviewer_keywords:
- ICLRErrorReportingManager::EndCustomDump method [.NET Framework hosting]
- EndCustomDump method [.NET Framework hosting]
ms.assetid: 88a5da04-8729-4108-82c4-af206a7d483e
topic_type: apiref
caps.latest.revision: "10"
author: rpetrusha
ms.author: ronpet
manager: wpickett
ms.openlocfilehash: 059ab01d3cc05bac84bb1a4cd8fffc7fc259ed60
ms.sourcegitcommit: 4f3fef493080a43e70e951223894768d36ce430a
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/21/2017
---
# <a name="iclrerrorreportingmanagerendcustomdump-method"></a><span data-ttu-id="3a699-102">ICLRErrorReportingManager::EndCustomDump 메서드</span><span class="sxs-lookup"><span data-stu-id="3a699-102">ICLRErrorReportingManager::EndCustomDump Method</span></span>
<span data-ttu-id="3a699-103">호출 하 여 이전에 지정 된 사용자 지정 스택 덤프 구성을 제거는 [iclrerrorreportingmanager:: Begincustomdump](../../../../docs/framework/unmanaged-api/hosting/iclrerrorreportingmanager-begincustomdump-method.md) 메서드.</span><span class="sxs-lookup"><span data-stu-id="3a699-103">Removes the custom stack dump configuration that was specified in an earlier call to the [ICLRErrorReportingManager::BeginCustomDump](../../../../docs/framework/unmanaged-api/hosting/iclrerrorreportingmanager-begincustomdump-method.md) method.</span></span>  
  
## <a name="syntax"></a><span data-ttu-id="3a699-104">구문</span><span class="sxs-lookup"><span data-stu-id="3a699-104">Syntax</span></span>  
  
```  
HRESULT EndCustomDump ();  
```  
  
## <a name="return-value"></a><span data-ttu-id="3a699-105">반환 값</span><span class="sxs-lookup"><span data-stu-id="3a699-105">Return Value</span></span>  
  
|<span data-ttu-id="3a699-106">HRESULT</span><span class="sxs-lookup"><span data-stu-id="3a699-106">HRESULT</span></span>|<span data-ttu-id="3a699-107">설명</span><span class="sxs-lookup"><span data-stu-id="3a699-107">Description</span></span>|  
|-------------|-----------------|  
|<span data-ttu-id="3a699-108">S_OK</span><span class="sxs-lookup"><span data-stu-id="3a699-108">S_OK</span></span>|<span data-ttu-id="3a699-109">`EndCustomDump`성공적으로 반환 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a699-109">`EndCustomDump` returned successfully.</span></span>|  
|<span data-ttu-id="3a699-110">HOST_E_CLRNOTAVAILABLE</span><span class="sxs-lookup"><span data-stu-id="3a699-110">HOST_E_CLRNOTAVAILABLE</span></span>|<span data-ttu-id="3a699-111">공용 언어 런타임 (CLR) 프로세스에 로드 되지 않았습니다 또는 CLR 중인 상태를 관리 코드를 실행 하거나 호출을 처리할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="3a699-111">The common language runtime (CLR) has not been loaded into a process, or the CLR is in a state in which it cannot run managed code or process the call successfully.</span></span>|  
|<span data-ttu-id="3a699-112">HOST_E_TIMEOUT</span><span class="sxs-lookup"><span data-stu-id="3a699-112">HOST_E_TIMEOUT</span></span>|<span data-ttu-id="3a699-113">호출 시간이 초과 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="3a699-113">The call timed out.</span></span>|  
|<span data-ttu-id="3a699-114">HOST_E_NOT_OWNER</span><span class="sxs-lookup"><span data-stu-id="3a699-114">HOST_E_NOT_OWNER</span></span>|<span data-ttu-id="3a699-115">호출자에 게 잠금을 소유 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="3a699-115">The caller does not own the lock.</span></span>|  
|<span data-ttu-id="3a699-116">HOST_E_ABANDONED</span><span class="sxs-lookup"><span data-stu-id="3a699-116">HOST_E_ABANDONED</span></span>|<span data-ttu-id="3a699-117">차단 된 스레드 이벤트 취소 되었습니다 또는 파이버가 기다리던 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a699-117">An event was canceled while a blocked thread or fiber was waiting on it.</span></span>|  
|<span data-ttu-id="3a699-118">E_FAIL</span><span class="sxs-lookup"><span data-stu-id="3a699-118">E_FAIL</span></span>|<span data-ttu-id="3a699-119">알 수 없는 치명적인 오류가 발생 했습니다.</span><span class="sxs-lookup"><span data-stu-id="3a699-119">An unknown catastrophic failure occurred.</span></span> <span data-ttu-id="3a699-120">E_FAIL을 반환 하는 메서드 후 CLR을 프로세스 내에서 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="3a699-120">After a method returns E_FAIL, the CLR is no longer usable within the process.</span></span> <span data-ttu-id="3a699-121">호스팅 방법에 대 한 후속 호출 HOST_E_CLRNOTAVAILABLE를 반환 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a699-121">Subsequent calls to hosting methods return HOST_E_CLRNOTAVAILABLE.</span></span>|  
  
## <a name="remarks"></a><span data-ttu-id="3a699-122">설명</span><span class="sxs-lookup"><span data-stu-id="3a699-122">Remarks</span></span>  
 <span data-ttu-id="3a699-123">`EndCustomDump` 메서드를 호출 하 여 이전으로 설정 된 사용자 지정 스택 덤프 구성을 지웁니다는 `BeginCustomDump` 메서드 및 연결 된 모든 상태를 해제 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a699-123">The `EndCustomDump` method clears the custom stack dump configuration set by an earlier call to the `BeginCustomDump` method and frees any associated state.</span></span> <span data-ttu-id="3a699-124">사용자 지정 스택 덤프 완료 된 후 호출 되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a699-124">It should be called after the custom stack dump is complete.</span></span>  
  
> [!IMPORTANT]
>  <span data-ttu-id="3a699-125">호출 하지 못하면 `EndCustomDump` 하면 메모리 누수를 발생 시킵니다.</span><span class="sxs-lookup"><span data-stu-id="3a699-125">Failure to call `EndCustomDump` causes memory to leak.</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="3a699-126">요구 사항</span><span class="sxs-lookup"><span data-stu-id="3a699-126">Requirements</span></span>  
 <span data-ttu-id="3a699-127">**플랫폼:** 참조 [시스템 요구 사항](../../../../docs/framework/get-started/system-requirements.md)합니다.</span><span class="sxs-lookup"><span data-stu-id="3a699-127">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="3a699-128">**헤더:** MSCorEE.h</span><span class="sxs-lookup"><span data-stu-id="3a699-128">**Header:** MSCorEE.h</span></span>  
  
 <span data-ttu-id="3a699-129">**라이브러리:** MSCorEE.dll에 리소스로 포함</span><span class="sxs-lookup"><span data-stu-id="3a699-129">**Library:** Included as a resource in MSCorEE.dll</span></span>  
  
 <span data-ttu-id="3a699-130">**.NET framework 버전:**[!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="3a699-130">**.NET Framework Versions:** [!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="3a699-131">참고 항목</span><span class="sxs-lookup"><span data-stu-id="3a699-131">See Also</span></span>  
 [<span data-ttu-id="3a699-132">CustomDumpItem 구조체</span><span class="sxs-lookup"><span data-stu-id="3a699-132">CustomDumpItem Structure</span></span>](../../../../docs/framework/unmanaged-api/hosting/customdumpitem-structure.md)  
 [<span data-ttu-id="3a699-133">ECustomDumpFlavor 열거형</span><span class="sxs-lookup"><span data-stu-id="3a699-133">ECustomDumpFlavor Enumeration</span></span>](../../../../docs/framework/unmanaged-api/hosting/ecustomdumpflavor-enumeration.md)  
 [<span data-ttu-id="3a699-134">ICLRErrorReportingManager 인터페이스</span><span class="sxs-lookup"><span data-stu-id="3a699-134">ICLRErrorReportingManager Interface</span></span>](../../../../docs/framework/unmanaged-api/hosting/iclrerrorreportingmanager-interface.md)