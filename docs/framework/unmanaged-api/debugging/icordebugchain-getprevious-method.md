---
title: "ICorDebugChain::GetPrevious 메서드"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: ICorDebugChain.GetPrevious
api_location: mscordbi.dll
api_type: COM
f1_keywords: ICorDebugChain::GetPrevious
helpviewer_keywords:
- ICorDebugChain::GetPrevious method [.NET Framework debugging]
- GetPrevious method [.NET Framework debugging]
ms.assetid: 58eed4c8-d80c-4c6a-a875-967a90dd926c
topic_type: apiref
caps.latest.revision: "14"
author: rpetrusha
ms.author: ronpet
manager: wpickett
ms.openlocfilehash: 1203aa4a6e35574c1d026ddc05cac810fed5b78b
ms.sourcegitcommit: bd1ef61f4bb794b25383d3d72e71041a5ced172e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/18/2017
---
# <a name="icordebugchaingetprevious-method"></a><span data-ttu-id="43571-102">ICorDebugChain::GetPrevious 메서드</span><span class="sxs-lookup"><span data-stu-id="43571-102">ICorDebugChain::GetPrevious Method</span></span>
<span data-ttu-id="43571-103">스레드에 대 한 이전 프레임 체인을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="43571-103">Gets the previous chain of frames for the thread.</span></span>  
  
## <a name="syntax"></a><span data-ttu-id="43571-104">구문</span><span class="sxs-lookup"><span data-stu-id="43571-104">Syntax</span></span>  
  
```  
HRESULT GetPrevious (  
    [out] ICorDebugChain     **ppChain  
);  
```  
  
#### <a name="parameters"></a><span data-ttu-id="43571-105">매개 변수</span><span class="sxs-lookup"><span data-stu-id="43571-105">Parameters</span></span>  
 `ppChain`  
 <span data-ttu-id="43571-106">[out] 이 스레드에 대 한 프레임의 이전 체인을 나타내는 ICorDebugChain 개체의 주소에 대 한 포인터입니다.</span><span class="sxs-lookup"><span data-stu-id="43571-106">[out] A pointer to the address of an ICorDebugChain object that represents the previous chain of frames for this thread.</span></span> <span data-ttu-id="43571-107">이 체인은 첫 번째 체인 경우 `ppChain` null입니다.</span><span class="sxs-lookup"><span data-stu-id="43571-107">If this chain is the first chain, `ppChain` is null.</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="43571-108">요구 사항</span><span class="sxs-lookup"><span data-stu-id="43571-108">Requirements</span></span>  
 <span data-ttu-id="43571-109">**플랫폼:** 참조 [시스템 요구 사항](../../../../docs/framework/get-started/system-requirements.md)합니다.</span><span class="sxs-lookup"><span data-stu-id="43571-109">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="43571-110">**헤더:** CorDebug.idl, CorDebug.h</span><span class="sxs-lookup"><span data-stu-id="43571-110">**Header:** CorDebug.idl, CorDebug.h</span></span>  
  
 <span data-ttu-id="43571-111">**라이브러리:** CorGuids.lib</span><span class="sxs-lookup"><span data-stu-id="43571-111">**Library:** CorGuids.lib</span></span>  
  
 <span data-ttu-id="43571-112">**.NET framework 버전:**[!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="43571-112">**.NET Framework Versions:** [!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]</span></span>