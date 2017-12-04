---
title: "GetHashFromFile 함수"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: GetHashFromFile
api_location: mscoree.dll
api_type: DLLExport
f1_keywords: GetHashFromFile
helpviewer_keywords: GetHashFromFile function [.NET Framework strong naming]
ms.assetid: b3c526a4-8fb4-4ad6-b6af-42ce9c06492e
topic_type: apiref
caps.latest.revision: "17"
author: rpetrusha
ms.author: ronpet
manager: wpickett
ms.openlocfilehash: 3c8e84881822cbafa8c43c3669f7522c390d5c5e
ms.sourcegitcommit: 4f3fef493080a43e70e951223894768d36ce430a
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/21/2017
---
# <a name="gethashfromfile-function"></a><span data-ttu-id="dd344-102">GetHashFromFile 함수</span><span class="sxs-lookup"><span data-stu-id="dd344-102">GetHashFromFile Function</span></span>
<span data-ttu-id="dd344-103">지정된 된 파일의 내용에 대 한 해시를 생성 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd344-103">Generates a hash over the contents of the specified file.</span></span>  
  
 <span data-ttu-id="dd344-104">이 함수는 더 이상 사용 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="dd344-104">This function has been deprecated.</span></span> <span data-ttu-id="dd344-105">사용 하 여 [iclrstrongname:: Gethashfromfile](../../../../docs/framework/unmanaged-api/hosting/iclrstrongname-gethashfromfile-method.md) 메서드 대신 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd344-105">Use the [ICLRStrongName::GetHashFromFile](../../../../docs/framework/unmanaged-api/hosting/iclrstrongname-gethashfromfile-method.md) method instead.</span></span>  
  
## <a name="syntax"></a><span data-ttu-id="dd344-106">구문</span><span class="sxs-lookup"><span data-stu-id="dd344-106">Syntax</span></span>  
  
```  
HRESULT GetHashFromFile (  
    [in]  LPCSTR   szFilePath,  
    [in, out] unsigned int   *piHashAlg,   
    [out] BYTE     *pbHash,      
    [in]  DWORD    cchHash,      
    [out] DWORD    *pchHash  
);  
```  
  
#### <a name="parameters"></a><span data-ttu-id="dd344-107">매개 변수</span><span class="sxs-lookup"><span data-stu-id="dd344-107">Parameters</span></span>  
 `szFilePath`  
 <span data-ttu-id="dd344-108">[in] 해시 파일의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="dd344-108">[in] The name of the file to hash.</span></span>  
  
 `piHashAlg`  
 <span data-ttu-id="dd344-109">[out에서] 해시를 생성할 때 사용 하는 알고리즘입니다.</span><span class="sxs-lookup"><span data-stu-id="dd344-109">[in, out] The algorithm to use when generating the hash.</span></span> <span data-ttu-id="dd344-110">유효한 알고리즘은 Win32 CryptoAPI에 의해 정의 된 것입니다.</span><span class="sxs-lookup"><span data-stu-id="dd344-110">Valid algorithms are those defined by the Win32 CryptoAPI.</span></span> <span data-ttu-id="dd344-111">경우 `piHashAlg` CALG_SHA-1은 사용 되는 기본 알고리즘 0으로 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="dd344-111">If `piHashAlg` is set to 0, the default algorithm CALG_SHA-1 is used.</span></span>  
  
 `pbHash`  
 <span data-ttu-id="dd344-112">[out] 생성된 된 해시를 포함 하는 바이트 배열입니다.</span><span class="sxs-lookup"><span data-stu-id="dd344-112">[out] A byte array containing the generated hash.</span></span>  
  
 `cchHash`  
 <span data-ttu-id="dd344-113">[in] 버퍼의 최대 크기는 `pbHash` 를 가리킵니다.</span><span class="sxs-lookup"><span data-stu-id="dd344-113">[in] The maximum size of the buffer that `pbHash` points to.</span></span>  
  
 `pchHash`  
 <span data-ttu-id="dd344-114">[out] 반환 된 바이트 단위로 크기 `pbHash`합니다.</span><span class="sxs-lookup"><span data-stu-id="dd344-114">[out] The size, in bytes, of the returned `pbHash`.</span></span>  
  
## <a name="remarks"></a><span data-ttu-id="dd344-115">설명</span><span class="sxs-lookup"><span data-stu-id="dd344-115">Remarks</span></span>  
 <span data-ttu-id="dd344-116">이 함수는 동일 [GetHashFromFileW](../../../../docs/framework/unmanaged-api/strong-naming/gethashfromfilew-function.md)제외 하 고 파일 이름 지정이 유니코드 대신 ANSI 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd344-116">This function is the same as [GetHashFromFileW](../../../../docs/framework/unmanaged-api/strong-naming/gethashfromfilew-function.md), except that the file name specification is ANSI instead of Unicode.</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="dd344-117">요구 사항</span><span class="sxs-lookup"><span data-stu-id="dd344-117">Requirements</span></span>  
 <span data-ttu-id="dd344-118">**플랫폼:** 참조 [시스템 요구 사항](../../../../docs/framework/get-started/system-requirements.md)합니다.</span><span class="sxs-lookup"><span data-stu-id="dd344-118">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="dd344-119">**헤더:** StrongName.h</span><span class="sxs-lookup"><span data-stu-id="dd344-119">**Header:** StrongName.h</span></span>  
  
 <span data-ttu-id="dd344-120">**라이브러리:** MsCorEE.dll에 리소스로 포함</span><span class="sxs-lookup"><span data-stu-id="dd344-120">**Library:** Included as a resource in MsCorEE.dll</span></span>  
  
 <span data-ttu-id="dd344-121">**.NET framework 버전:**[!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="dd344-121">**.NET Framework Versions:** [!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="dd344-122">참고 항목</span><span class="sxs-lookup"><span data-stu-id="dd344-122">See Also</span></span>  
 [<span data-ttu-id="dd344-123">GetHashFromFile 메서드</span><span class="sxs-lookup"><span data-stu-id="dd344-123">GetHashFromFile Method</span></span>](../../../../docs/framework/unmanaged-api/hosting/iclrstrongname-gethashfromfile-method.md)  
 [<span data-ttu-id="dd344-124">GetHashFromFileW 메서드</span><span class="sxs-lookup"><span data-stu-id="dd344-124">GetHashFromFileW Method</span></span>](../../../../docs/framework/unmanaged-api/hosting/iclrstrongname-gethashfromfilew-method.md)  
 [<span data-ttu-id="dd344-125">ICLRStrongName 인터페이스</span><span class="sxs-lookup"><span data-stu-id="dd344-125">ICLRStrongName Interface</span></span>](../../../../docs/framework/unmanaged-api/hosting/iclrstrongname-interface.md)