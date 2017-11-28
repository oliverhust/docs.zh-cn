---
title: "ICorDebugThread::GetActiveChain 方法"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: ICorDebugThread.GetActiveChain
api_location: mscordbi.dll
api_type: COM
f1_keywords: ICorDebugThread::GetActiveChain
helpviewer_keywords:
- ICorDebugThread::GetActiveChain method [.NET Framework debugging]
- GetActiveChain method [.NET Framework debugging]
ms.assetid: f50de1f7-40ef-4949-b542-1d9a61f7bfef
topic_type: apiref
caps.latest.revision: "13"
author: rpetrusha
ms.author: ronpet
manager: wpickett
ms.openlocfilehash: f3f104933bc70682a531c0853cfc6eabcd357831
ms.sourcegitcommit: bd1ef61f4bb794b25383d3d72e71041a5ced172e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2017
---
# <a name="icordebugthreadgetactivechain-method"></a><span data-ttu-id="71941-102">ICorDebugThread::GetActiveChain 方法</span><span class="sxs-lookup"><span data-stu-id="71941-102">ICorDebugThread::GetActiveChain Method</span></span>
<span data-ttu-id="71941-103">获取此 ICorDebugThread 对象上的活动的 （最新） 堆栈链的接口指针。</span><span class="sxs-lookup"><span data-stu-id="71941-103">Gets an interface pointer to the active (most recent) stack chain on this ICorDebugThread object.</span></span>  
  
## <a name="syntax"></a><span data-ttu-id="71941-104">语法</span><span class="sxs-lookup"><span data-stu-id="71941-104">Syntax</span></span>  
  
```  
HRESULT GetActiveChain (  
    [out] ICorDebugChain **ppChain  
);  
```  
  
#### <a name="parameters"></a><span data-ttu-id="71941-105">参数</span><span class="sxs-lookup"><span data-stu-id="71941-105">Parameters</span></span>  
 `ppChain`  
 <span data-ttu-id="71941-106">[out]指向一个表示堆栈链的 ICorDebugChain 对象的地址的指针。</span><span class="sxs-lookup"><span data-stu-id="71941-106">[out] A pointer to the address of an ICorDebugChain object that represents the stack chain.</span></span>  
  
## <a name="remarks"></a><span data-ttu-id="71941-107">备注</span><span class="sxs-lookup"><span data-stu-id="71941-107">Remarks</span></span>  
 <span data-ttu-id="71941-108">`ppChain`参数是没有堆栈链当前处于活动状态的情况下为 null。</span><span class="sxs-lookup"><span data-stu-id="71941-108">The `ppChain` parameter is null if no stack chain is currently active.</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="71941-109">要求</span><span class="sxs-lookup"><span data-stu-id="71941-109">Requirements</span></span>  
 <span data-ttu-id="71941-110">**平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。</span><span class="sxs-lookup"><span data-stu-id="71941-110">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="71941-111">**标头：** CorDebug.idl、 CorDebug.h</span><span class="sxs-lookup"><span data-stu-id="71941-111">**Header:** CorDebug.idl, CorDebug.h</span></span>  
  
 <span data-ttu-id="71941-112">**库：** CorGuids.lib</span><span class="sxs-lookup"><span data-stu-id="71941-112">**Library:** CorGuids.lib</span></span>  
  
 <span data-ttu-id="71941-113">**.NET framework 版本：**[!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="71941-113">**.NET Framework Versions:** [!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]</span></span>