---
title: "ICorDebugRegisterSet2 인터페이스"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: ICorDebugRegisterSet2
api_location: mscordbi.dll
api_type: COM
f1_keywords: ICorDebugRegisterSet2
helpviewer_keywords: ICorDebugRegisterSet2 interface [.NET Framework debugging]
ms.assetid: d7fbccbf-3b6b-4db8-a96d-768e1cb6b1a6
topic_type: apiref
caps.latest.revision: "14"
author: rpetrusha
ms.author: ronpet
manager: wpickett
ms.openlocfilehash: 26967f50ded62f935a705c25eed58314b77bedd8
ms.sourcegitcommit: 4f3fef493080a43e70e951223894768d36ce430a
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/21/2017
---
# <a name="icordebugregisterset2-interface"></a><span data-ttu-id="021b4-102">ICorDebugRegisterSet2 인터페이스</span><span class="sxs-lookup"><span data-stu-id="021b4-102">ICorDebugRegisterSet2 Interface</span></span>
<span data-ttu-id="021b4-103">기능을 확장 된 [ICorDebugRegisterSet](../../../../docs/framework/unmanaged-api/debugging/icordebugregisterset-interface.md) 64 개 이상의 레지스터가 있는 하드웨어 플랫폼에 대 한 인터페이스입니다.</span><span class="sxs-lookup"><span data-stu-id="021b4-103">Extends the capabilities of the [ICorDebugRegisterSet](../../../../docs/framework/unmanaged-api/debugging/icordebugregisterset-interface.md) interface for hardware platforms that have more than 64 registers.</span></span>  
  
## <a name="methods"></a><span data-ttu-id="021b4-104">메서드</span><span class="sxs-lookup"><span data-stu-id="021b4-104">Methods</span></span>  
  
|<span data-ttu-id="021b4-105">메서드</span><span class="sxs-lookup"><span data-stu-id="021b4-105">Method</span></span>|<span data-ttu-id="021b4-106">설명</span><span class="sxs-lookup"><span data-stu-id="021b4-106">Description</span></span>|  
|------------|-----------------|  
|[<span data-ttu-id="021b4-107">GetRegisters 메서드</span><span class="sxs-lookup"><span data-stu-id="021b4-107">GetRegisters Method</span></span>](../../../../docs/framework/unmanaged-api/debugging/icordebugregisterset2-getregisters-method.md)|<span data-ttu-id="021b4-108">(현재 코드를 실행 하는 컴퓨터)에서 각 레지스터의 값을 가져옵니다는 비트 마스크에 의해 지정 된 합니다.</span><span class="sxs-lookup"><span data-stu-id="021b4-108">Gets the value of each register (on the computer that is currently executing code) that is specified by the bit mask.</span></span>|  
|[<span data-ttu-id="021b4-109">GetRegistersAvailable 메서드</span><span class="sxs-lookup"><span data-stu-id="021b4-109">GetRegistersAvailable Method</span></span>](../../../../docs/framework/unmanaged-api/debugging/icordebugregisterset2-getregistersavailable-method.md)|<span data-ttu-id="021b4-110">사용 가능한 레지스터의 비트맵을 제공 하는 바이트의 배열을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="021b4-110">Gets an array of bytes that provides a bitmap of the available registers.</span></span>|  
|[<span data-ttu-id="021b4-111">SetRegisters 메서드</span><span class="sxs-lookup"><span data-stu-id="021b4-111">SetRegisters Method</span></span>](../../../../docs/framework/unmanaged-api/debugging/icordebugregisterset2-setregisters-method.md)|<span data-ttu-id="021b4-112">.NET Framework 버전 2.0에서에서 구현 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="021b4-112">Not implemented in the .NET Framework version 2.0.</span></span>|  
  
## <a name="remarks"></a><span data-ttu-id="021b4-113">설명</span><span class="sxs-lookup"><span data-stu-id="021b4-113">Remarks</span></span>  
  
> [!NOTE]
>  <span data-ttu-id="021b4-114">이 인터페이스는 크로스 시스템 또는 크로스 프로세스 원격 호출을 지원하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="021b4-114">This interface does not support being called remotely, either cross-machine or cross-process.</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="021b4-115">요구 사항</span><span class="sxs-lookup"><span data-stu-id="021b4-115">Requirements</span></span>  
 <span data-ttu-id="021b4-116">**플랫폼:** 참조 [시스템 요구 사항](../../../../docs/framework/get-started/system-requirements.md)합니다.</span><span class="sxs-lookup"><span data-stu-id="021b4-116">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="021b4-117">**헤더:** CorDebug.idl, CorDebug.h</span><span class="sxs-lookup"><span data-stu-id="021b4-117">**Header:** CorDebug.idl, CorDebug.h</span></span>  
  
 <span data-ttu-id="021b4-118">**라이브러리:** CorGuids.lib</span><span class="sxs-lookup"><span data-stu-id="021b4-118">**Library:** CorGuids.lib</span></span>  
  
 <span data-ttu-id="021b4-119">**.NET framework 버전:**[!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="021b4-119">**.NET Framework Versions:** [!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="021b4-120">참고 항목</span><span class="sxs-lookup"><span data-stu-id="021b4-120">See Also</span></span>  
 [<span data-ttu-id="021b4-121">디버깅 인터페이스</span><span class="sxs-lookup"><span data-stu-id="021b4-121">Debugging Interfaces</span></span>](../../../../docs/framework/unmanaged-api/debugging/debugging-interfaces.md)  
 [<span data-ttu-id="021b4-122">ICorDebugRegisterSet 인터페이스</span><span class="sxs-lookup"><span data-stu-id="021b4-122">ICorDebugRegisterSet Interface</span></span>](../../../../docs/framework/unmanaged-api/debugging/icordebugregisterset-interface.md)