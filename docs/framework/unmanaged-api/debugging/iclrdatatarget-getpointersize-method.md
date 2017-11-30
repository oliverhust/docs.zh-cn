---
title: "ICLRDataTarget::GetPointerSize 方法"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: ICLRDataTarget.GetPointerSize
api_location: mscordbi.dll
api_type: COM
f1_keywords: ICLRDataTarget::GetPointerSize
helpviewer_keywords:
- GetPointerSize method [.NET Framework debugging]
- ICLRDataTarget::GetPointerSize method [.NET Framework debugging]
ms.assetid: 51d9f4a4-81a7-4527-8537-5212bdb05c70
topic_type: apiref
caps.latest.revision: "11"
author: rpetrusha
ms.author: ronpet
manager: wpickett
ms.openlocfilehash: c71f093bd663fb2622dbfc212671fad8f19ca4a9
ms.sourcegitcommit: bd1ef61f4bb794b25383d3d72e71041a5ced172e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2017
---
# <a name="iclrdatatargetgetpointersize-method"></a><span data-ttu-id="180a0-102">ICLRDataTarget::GetPointerSize 方法</span><span class="sxs-lookup"><span data-stu-id="180a0-102">ICLRDataTarget::GetPointerSize Method</span></span>
<span data-ttu-id="180a0-103">获取大小，以字节为单位，则目标进程将使用与指针类型。</span><span class="sxs-lookup"><span data-stu-id="180a0-103">Gets the size, in bytes, of the pointer type that the target process uses.</span></span> <span data-ttu-id="180a0-104">由公共语言运行时数据访问服务调用此方法。</span><span class="sxs-lookup"><span data-stu-id="180a0-104">This method is called by the common language runtime data access services.</span></span>  
  
## <a name="syntax"></a><span data-ttu-id="180a0-105">语法</span><span class="sxs-lookup"><span data-stu-id="180a0-105">Syntax</span></span>  
  
```  
HRESULT GetPointerSize (  
    [out] ULONG32     *pointerSize  
);  
```  
  
#### <a name="parameters"></a><span data-ttu-id="180a0-106">参数</span><span class="sxs-lookup"><span data-stu-id="180a0-106">Parameters</span></span>  
 `pointerSize`  
 <span data-ttu-id="180a0-107">[out]指向一个整数值，指定大小，以字节为单位，在目标进程的指针的指针。</span><span class="sxs-lookup"><span data-stu-id="180a0-107">[out] A pointer to an integer value that specifies the size, in bytes, of a pointer on the target process.</span></span>  
  
## <a name="remarks"></a><span data-ttu-id="180a0-108">备注</span><span class="sxs-lookup"><span data-stu-id="180a0-108">Remarks</span></span>  
 <span data-ttu-id="180a0-109">此方法由调试应用程序的编写器实现。</span><span class="sxs-lookup"><span data-stu-id="180a0-109">This method is implemented by the writer of the debugging application.</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="180a0-110">要求</span><span class="sxs-lookup"><span data-stu-id="180a0-110">Requirements</span></span>  
 <span data-ttu-id="180a0-111">**平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。</span><span class="sxs-lookup"><span data-stu-id="180a0-111">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="180a0-112">**标头：** ClrData.idl、 ClrData.h</span><span class="sxs-lookup"><span data-stu-id="180a0-112">**Header:** ClrData.idl, ClrData.h</span></span>  
  
 <span data-ttu-id="180a0-113">**库：** CorGuids.lib</span><span class="sxs-lookup"><span data-stu-id="180a0-113">**Library:** CorGuids.lib</span></span>  
  
 <span data-ttu-id="180a0-114">**.NET framework 版本：**[!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="180a0-114">**.NET Framework Versions:** [!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="180a0-115">另请参阅</span><span class="sxs-lookup"><span data-stu-id="180a0-115">See Also</span></span>  
 [<span data-ttu-id="180a0-116">ICLRDataTarget 接口</span><span class="sxs-lookup"><span data-stu-id="180a0-116">ICLRDataTarget Interface</span></span>](../../../../docs/framework/unmanaged-api/debugging/iclrdatatarget-interface.md)