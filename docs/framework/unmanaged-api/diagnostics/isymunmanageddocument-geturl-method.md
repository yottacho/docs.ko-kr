---
title: "ISymUnmanagedDocument::GetURL 메서드"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: ISymUnmanagedDocument.GetURL
api_location: diasymreader.dll
api_type: COM
f1_keywords: ISymUnmanagedDocument::GetURL
helpviewer_keywords:
- GetURL method [.NET Framework debugging]
- ISymUnmanagedDocument::GetURL method [.NET Framework debugging]
ms.assetid: 60600178-c2b5-4cab-b3a5-f0f61acebaf1
topic_type: apiref
caps.latest.revision: "9"
author: mairaw
ms.author: mairaw
manager: wpickett
ms.openlocfilehash: 591383fee2f9b22a00956193555c719e72d722bb
ms.sourcegitcommit: bd1ef61f4bb794b25383d3d72e71041a5ced172e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/18/2017
---
# <a name="isymunmanageddocumentgeturl-method"></a><span data-ttu-id="28d42-102">ISymUnmanagedDocument::GetURL 메서드</span><span class="sxs-lookup"><span data-stu-id="28d42-102">ISymUnmanagedDocument::GetURL Method</span></span>
<span data-ttu-id="28d42-103">이 문서에 대 한 uniform resource locator (URL)를 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="28d42-103">Returns the uniform resource locator (URL) for this document.</span></span>  
  
## <a name="syntax"></a><span data-ttu-id="28d42-104">구문</span><span class="sxs-lookup"><span data-stu-id="28d42-104">Syntax</span></span>  
  
```  
HRESULT GetURL(  
    [in]  ULONG32  cchUrl,  
    [out] ULONG32  *pcchUrl,  
    [out, size_is(cchUrl), length_is(*pcchUrl)] WCHAR szUrl[]);  
```  
  
#### <a name="parameters"></a><span data-ttu-id="28d42-105">매개 변수</span><span class="sxs-lookup"><span data-stu-id="28d42-105">Parameters</span></span>  
 `cchUrl`  
 <span data-ttu-id="28d42-106">[in] 크기 문자의는 `szURL` 버퍼입니다.</span><span class="sxs-lookup"><span data-stu-id="28d42-106">[in] The size, in characters, of the `szURL` buffer.</span></span>  
  
 `pcchUrl`  
 <span data-ttu-id="28d42-107">[out] Null 종료를 포함 하는 URL의 크기를 받는 변수에 대 한 포인터입니다.</span><span class="sxs-lookup"><span data-stu-id="28d42-107">[out] A pointer to a variable that receives the size of the URL, including the null termination.</span></span>  
  
 `szUrl`  
 <span data-ttu-id="28d42-108">[out] URL을 포함 하는 버퍼입니다.</span><span class="sxs-lookup"><span data-stu-id="28d42-108">[out] The buffer containing the URL.</span></span>  
  
## <a name="return-value"></a><span data-ttu-id="28d42-109">반환 값</span><span class="sxs-lookup"><span data-stu-id="28d42-109">Return Value</span></span>  
 <span data-ttu-id="28d42-110">메서드가 성공 하면 s_ok이 고 그렇지 않으면 오류 코드가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="28d42-110">S_OK if the method succeeds; otherwise, an error code.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="28d42-111">참고 항목</span><span class="sxs-lookup"><span data-stu-id="28d42-111">See Also</span></span>  
 [<span data-ttu-id="28d42-112">ISymUnmanagedDocument 인터페이스</span><span class="sxs-lookup"><span data-stu-id="28d42-112">ISymUnmanagedDocument Interface</span></span>](../../../../docs/framework/unmanaged-api/diagnostics/isymunmanageddocument-interface.md)