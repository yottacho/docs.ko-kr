---
title: "ICLRRuntimeInfo::GetProcAddress 메서드"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: ICLRRuntimeInfo.GetProcAddress
api_location: mscoree.dll
api_type: COM
f1_keywords: ICLRRuntimeInfo::GetProcAddress
helpviewer_keywords:
- GetProcAddress method [.NET Framework hosting]
- ICLRRuntimeInfo::GetProcAddress method [.NET Framework hosting]
ms.assetid: a7732bfc-689a-4926-88fd-4f81e6f9ed78
topic_type: apiref
caps.latest.revision: "10"
author: rpetrusha
ms.author: ronpet
manager: wpickett
ms.openlocfilehash: e1b8af06a52a3961bb3e551375350dee849343b3
ms.sourcegitcommit: 4f3fef493080a43e70e951223894768d36ce430a
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/21/2017
---
# <a name="iclrruntimeinfogetprocaddress-method"></a><span data-ttu-id="0e670-102">ICLRRuntimeInfo::GetProcAddress 메서드</span><span class="sxs-lookup"><span data-stu-id="0e670-102">ICLRRuntimeInfo::GetProcAddress Method</span></span>
<span data-ttu-id="0e670-103">이 인터페이스와 연결 된 공용 언어 런타임 (CLR)에서 내보낸 지정된 된 함수 주소를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="0e670-103">Gets the address of a specified function that was exported from the common language runtime (CLR) associated with this interface.</span></span>  
  
 <span data-ttu-id="0e670-104">이 메서드를 대체는 [GetRealProcAddress](../../../../docs/framework/unmanaged-api/hosting/getrealprocaddress-function.md) 함수입니다.</span><span class="sxs-lookup"><span data-stu-id="0e670-104">This method supersedes the [GetRealProcAddress](../../../../docs/framework/unmanaged-api/hosting/getrealprocaddress-function.md) function.</span></span>  
  
## <a name="syntax"></a><span data-ttu-id="0e670-105">구문</span><span class="sxs-lookup"><span data-stu-id="0e670-105">Syntax</span></span>  
  
```  
HRESULT GetProcAddress(  
     [in]  LPCSTR pszProcName,  
     [out, retval] LPVOID *ppProc);  
```  
  
#### <a name="parameters"></a><span data-ttu-id="0e670-106">매개 변수</span><span class="sxs-lookup"><span data-stu-id="0e670-106">Parameters</span></span>  
 `pszProcName`  
 <span data-ttu-id="0e670-107">[in] 내보낸 함수의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="0e670-107">[in] The name of the exported function.</span></span>  
  
 `ppProc`  
 <span data-ttu-id="0e670-108">[out] 내보낸 함수의 주소입니다.</span><span class="sxs-lookup"><span data-stu-id="0e670-108">[out] The address of the exported function.</span></span>  
  
## <a name="return-value"></a><span data-ttu-id="0e670-109">반환 값</span><span class="sxs-lookup"><span data-stu-id="0e670-109">Return Value</span></span>  
 <span data-ttu-id="0e670-110">이 메서드는 다음과 같은 특정 HRESULT뿐만 아니라 메서드 오류를 나타내는 HRESULT 오류도 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="0e670-110">This method returns the following specific HRESULTs as well as HRESULT errors that indicate method failure.</span></span>  
  
|<span data-ttu-id="0e670-111">HRESULT</span><span class="sxs-lookup"><span data-stu-id="0e670-111">HRESULT</span></span>|<span data-ttu-id="0e670-112">설명</span><span class="sxs-lookup"><span data-stu-id="0e670-112">Description</span></span>|  
|-------------|-----------------|  
|<span data-ttu-id="0e670-113">S_OK</span><span class="sxs-lookup"><span data-stu-id="0e670-113">S_OK</span></span>|<span data-ttu-id="0e670-114">메서드가 완료되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0e670-114">The method completed successfully.</span></span>|  
|<span data-ttu-id="0e670-115">E_POINTER</span><span class="sxs-lookup"><span data-stu-id="0e670-115">E_POINTER</span></span>|<span data-ttu-id="0e670-116">`pszProcName` 또는 `ppProc`이 null입니다.</span><span class="sxs-lookup"><span data-stu-id="0e670-116">`pszProcName` or `ppProc` is null.</span></span>|  
|<span data-ttu-id="0e670-117">CLR_E_SHIM_RUNTIMEEXPORT</span><span class="sxs-lookup"><span data-stu-id="0e670-117">CLR_E_SHIM_RUNTIMEEXPORT</span></span>|<span data-ttu-id="0e670-118">지정된 된 함수는 내보낸된 함수가 않습니다.</span><span class="sxs-lookup"><span data-stu-id="0e670-118">The specified function is not an exported function.</span></span>|  
  
## <a name="remarks"></a><span data-ttu-id="0e670-119">설명</span><span class="sxs-lookup"><span data-stu-id="0e670-119">Remarks</span></span>  
 <span data-ttu-id="0e670-120">이 메서드를 사용 하면 CLR 로드 되지만 초기화 되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="0e670-120">This method causes the CLR to be loaded but not initialized.</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="0e670-121">요구 사항</span><span class="sxs-lookup"><span data-stu-id="0e670-121">Requirements</span></span>  
 <span data-ttu-id="0e670-122">**플랫폼:** 참조 [시스템 요구 사항](../../../../docs/framework/get-started/system-requirements.md)합니다.</span><span class="sxs-lookup"><span data-stu-id="0e670-122">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="0e670-123">**헤더:** MetaHost.h</span><span class="sxs-lookup"><span data-stu-id="0e670-123">**Header:** MetaHost.h</span></span>  
  
 <span data-ttu-id="0e670-124">**라이브러리:** MSCorEE.dll에 리소스로 포함</span><span class="sxs-lookup"><span data-stu-id="0e670-124">**Library:** Included as a resource in MSCorEE.dll</span></span>  
  
 <span data-ttu-id="0e670-125">**.NET framework 버전:**[!INCLUDE[net_current_v40plus](../../../../includes/net-current-v40plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="0e670-125">**.NET Framework Versions:** [!INCLUDE[net_current_v40plus](../../../../includes/net-current-v40plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="0e670-126">참고 항목</span><span class="sxs-lookup"><span data-stu-id="0e670-126">See Also</span></span>  
 [<span data-ttu-id="0e670-127">ICLRRuntimeInfo 인터페이스</span><span class="sxs-lookup"><span data-stu-id="0e670-127">ICLRRuntimeInfo Interface</span></span>](../../../../docs/framework/unmanaged-api/hosting/iclrruntimeinfo-interface.md)  
 [<span data-ttu-id="0e670-128">호스팅 인터페이스</span><span class="sxs-lookup"><span data-stu-id="0e670-128">Hosting Interfaces</span></span>](../../../../docs/framework/unmanaged-api/hosting/hosting-interfaces.md)  
 [<span data-ttu-id="0e670-129">호스팅</span><span class="sxs-lookup"><span data-stu-id="0e670-129">Hosting</span></span>](../../../../docs/framework/unmanaged-api/hosting/index.md)