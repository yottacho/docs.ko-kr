---
title: "ICorProfilerCallback3 인터페이스"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: ICorProfilerCallback3
api_location: mscorwks.dll
api_type: COM
f1_keywords: ICorProfilerCallback3
helpviewer_keywords: ICorProfilerCallback3 interface [.NET Framework profiling]
ms.assetid: be83af41-3dec-4c77-8529-9dd6b8042af6
topic_type: apiref
caps.latest.revision: "10"
author: mairaw
ms.author: mairaw
manager: wpickett
ms.openlocfilehash: c62dfb9b44999309ab2be7dfdcdfba3bb5dde29c
ms.sourcegitcommit: 4f3fef493080a43e70e951223894768d36ce430a
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/21/2017
---
# <a name="icorprofilercallback3-interface"></a><span data-ttu-id="e7c7d-102">ICorProfilerCallback3 인터페이스</span><span class="sxs-lookup"><span data-stu-id="e7c7d-102">ICorProfilerCallback3 Interface</span></span>
<span data-ttu-id="e7c7d-103">공용 언어 런타임 (CLR) 사용 하 여 통신 하는 콜백 메서드를 연결 및 분리를 프로파일러에 상태 정보를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="e7c7d-103">Provides callback methods that the common language runtime (CLR) uses to communicate attach and detach state information to the profiler.</span></span>  
  
## <a name="methods"></a><span data-ttu-id="e7c7d-104">메서드</span><span class="sxs-lookup"><span data-stu-id="e7c7d-104">Methods</span></span>  
  
|<span data-ttu-id="e7c7d-105">메서드</span><span class="sxs-lookup"><span data-stu-id="e7c7d-105">Method</span></span>|<span data-ttu-id="e7c7d-106">설명</span><span class="sxs-lookup"><span data-stu-id="e7c7d-106">Description</span></span>|  
|------------|-----------------|  
|[<span data-ttu-id="e7c7d-107">InitializeForAttach 메서드</span><span class="sxs-lookup"><span data-stu-id="e7c7d-107">InitializeForAttach Method</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback3-initializeforattach-method.md)|<span data-ttu-id="e7c7d-108">프로파일러가 연결 작업 후 해당 상태를 초기화할 수 있도록 CLR에서 호출 됩니다.</span><span class="sxs-lookup"><span data-stu-id="e7c7d-108">Called by the CLR to give the profiler an opportunity to initialize its state after an attach operation.</span></span>|  
|[<span data-ttu-id="e7c7d-109">ProfilerAttachComplete 메서드</span><span class="sxs-lookup"><span data-stu-id="e7c7d-109">ProfilerAttachComplete Method</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback3-profilerattachcomplete-method.md)|<span data-ttu-id="e7c7d-110">프로파일러가 이제 후속 메서드를 호출할 수 있도록 나타내기 위해 CLR에 의해 호출 됩니다.</span><span class="sxs-lookup"><span data-stu-id="e7c7d-110">Called by the CLR to indicate that the profiler can now call the catch-up methods.</span></span>|  
|[<span data-ttu-id="e7c7d-111">ProfilerDetachSucceeded 메서드</span><span class="sxs-lookup"><span data-stu-id="e7c7d-111">ProfilerDetachSucceeded Method</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback3-profilerdetachsucceeded-method.md)|<span data-ttu-id="e7c7d-112">CLR(공용 언어 런타임)이 프로파일러 DLL을 언로드한다고 프로파일러에 알립니다.</span><span class="sxs-lookup"><span data-stu-id="e7c7d-112">Notifies the profiler that the common language runtime (CLR) is about to unload the profiler DLL.</span></span>|  
  
## <a name="remarks"></a><span data-ttu-id="e7c7d-113">설명</span><span class="sxs-lookup"><span data-stu-id="e7c7d-113">Remarks</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="e7c7d-114">요구 사항</span><span class="sxs-lookup"><span data-stu-id="e7c7d-114">Requirements</span></span>  
 <span data-ttu-id="e7c7d-115">**플랫폼:** 참조 [시스템 요구 사항](../../../../docs/framework/get-started/system-requirements.md)합니다.</span><span class="sxs-lookup"><span data-stu-id="e7c7d-115">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="e7c7d-116">**헤더:** CorProf.idl, CorProf.h</span><span class="sxs-lookup"><span data-stu-id="e7c7d-116">**Header:** CorProf.idl, CorProf.h</span></span>  
  
 <span data-ttu-id="e7c7d-117">**라이브러리:** CorGuids.lib</span><span class="sxs-lookup"><span data-stu-id="e7c7d-117">**Library:** CorGuids.lib</span></span>  
  
 <span data-ttu-id="e7c7d-118">**.NET framework 버전:**[!INCLUDE[net_current_v40plus](../../../../includes/net-current-v40plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="e7c7d-118">**.NET Framework Versions:** [!INCLUDE[net_current_v40plus](../../../../includes/net-current-v40plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="e7c7d-119">참고 항목</span><span class="sxs-lookup"><span data-stu-id="e7c7d-119">See Also</span></span>  
 [<span data-ttu-id="e7c7d-120">프로 파일링 인터페이스</span><span class="sxs-lookup"><span data-stu-id="e7c7d-120">Profiling Interfaces</span></span>](../../../../docs/framework/unmanaged-api/profiling/profiling-interfaces.md)  
 [<span data-ttu-id="e7c7d-121">ICorProfilerInfo 인터페이스</span><span class="sxs-lookup"><span data-stu-id="e7c7d-121">ICorProfilerInfo Interface</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilerinfo-interface.md)  
 [<span data-ttu-id="e7c7d-122">ICorProfilerCallback2 인터페이스</span><span class="sxs-lookup"><span data-stu-id="e7c7d-122">ICorProfilerCallback2 Interface</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback2-interface.md)  
 [<span data-ttu-id="e7c7d-123">ICorProfilerCallback4 인터페이스</span><span class="sxs-lookup"><span data-stu-id="e7c7d-123">ICorProfilerCallback4 Interface</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback4-interface.md)