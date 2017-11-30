---
title: "IMetaDataImport::GetMemberProps 方法"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: IMetaDataImport.GetMemberProps
api_location: mscoree.dll
api_type: COM
f1_keywords: IMetaDataImport::GetMemberProps
helpviewer_keywords:
- IMetaDataImport::GetMemberProps method [.NET Framework metadata]
- GetMemberProps method [.NET Framework metadata]
ms.assetid: 42790918-4142-4938-b8f4-a56979a55846
topic_type: apiref
caps.latest.revision: "10"
author: mairaw
ms.author: mairaw
manager: wpickett
ms.openlocfilehash: b52d3130400310379c69eb0202217d1cd37ff18d
ms.sourcegitcommit: 4f3fef493080a43e70e951223894768d36ce430a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2017
---
# <a name="imetadataimportgetmemberprops-method"></a><span data-ttu-id="873ec-102">IMetaDataImport::GetMemberProps 方法</span><span class="sxs-lookup"><span data-stu-id="873ec-102">IMetaDataImport::GetMemberProps Method</span></span>
<span data-ttu-id="873ec-103">获取元数据信息，包括名称、 二进制签名和相对虚拟地址的<xref:System.Type>指定的元数据标记所引用的成员。</span><span class="sxs-lookup"><span data-stu-id="873ec-103">Gets metadata information, including the name, binary signature, and relative virtual address, of the <xref:System.Type> member referenced by the specified metadata token.</span></span>  
  
## <a name="syntax"></a><span data-ttu-id="873ec-104">语法</span><span class="sxs-lookup"><span data-stu-id="873ec-104">Syntax</span></span>  
  
```  
HRESULT GetMemberProps (  
   [in]  mdToken           mb,   
   [out] mdTypeDef         *pClass,  
   [out] LPWSTR            szMember,   
   [in]  ULONG             cchMember,   
   [out] ULONG             *pchMember,   
   [out] DWORD             *pdwAttr,  
   [out] PCCOR_SIGNATURE   *ppvSigBlob,   
   [out] ULONG             *pcbSigBlob,   
   [out] ULONG             *pulCodeRVA,   
   [out] DWORD             *pdwImplFlags,   
   [out] DWORD             *pdwCPlusTypeFlag,   
   [out] UVCP_CONSTANT     *ppValue,  
   [out] ULONG             *pcchValue  
);  
```  
  
#### <a name="parameters"></a><span data-ttu-id="873ec-105">参数</span><span class="sxs-lookup"><span data-stu-id="873ec-105">Parameters</span></span>  
 `mb`  
 <span data-ttu-id="873ec-106">[in]标记，用于引用要获取有关关联的元数据的成员。</span><span class="sxs-lookup"><span data-stu-id="873ec-106">[in] The token that references the member to get the associated metadata for.</span></span>  
  
 `pClass`  
 <span data-ttu-id="873ec-107">[out]指向表示的成员的类的元数据标记的指针。</span><span class="sxs-lookup"><span data-stu-id="873ec-107">[out] A pointer to the metadata token that represents the class of the member.</span></span>  
  
 `szMember`  
 <span data-ttu-id="873ec-108">[out]成员的名称。</span><span class="sxs-lookup"><span data-stu-id="873ec-108">[out] The name of the member.</span></span>  
  
 `cchMember`  
 <span data-ttu-id="873ec-109">[in]在宽字符为单位的大小`szMember`缓冲区。</span><span class="sxs-lookup"><span data-stu-id="873ec-109">[in] The size in wide characters of the `szMember` buffer.</span></span>  
  
 `pchMember`  
 <span data-ttu-id="873ec-110">[out]以宽字符为单位返回的名称的大小。</span><span class="sxs-lookup"><span data-stu-id="873ec-110">[out] The size in wide characters of the returned name.</span></span>  
  
 `pdwAttr`  
 <span data-ttu-id="873ec-111">[out]应用于的成员的任何标志值。</span><span class="sxs-lookup"><span data-stu-id="873ec-111">[out] Any flag values applied to the member.</span></span>  
  
 `ppvSigBlob`  
 <span data-ttu-id="873ec-112">[out]指向成员的二进制元数据签名的指针。</span><span class="sxs-lookup"><span data-stu-id="873ec-112">[out] A pointer to the binary metadata signature of the member.</span></span>  
  
 `pcbSigBlob`  
 <span data-ttu-id="873ec-113">[out]以字节为单位的大小`ppvSigBlob`。</span><span class="sxs-lookup"><span data-stu-id="873ec-113">[out] The size in bytes of `ppvSigBlob`.</span></span>  
  
 `pulCodeRVA`  
 <span data-ttu-id="873ec-114">[out]指向成员的相对虚拟地址的指针。</span><span class="sxs-lookup"><span data-stu-id="873ec-114">[out] A pointer to the relative virtual address of the member.</span></span>  
  
 `pdwImplFlags`  
 <span data-ttu-id="873ec-115">[out]成员关联的任何方法实现标志。</span><span class="sxs-lookup"><span data-stu-id="873ec-115">[out] Any method implementation flags associated with the member.</span></span>  
  
 `pdwCPlusTypeFlag`  
 <span data-ttu-id="873ec-116">[out]用于将标记的标志<xref:System.ValueType>。</span><span class="sxs-lookup"><span data-stu-id="873ec-116">[out] A flag that marks a <xref:System.ValueType>.</span></span>  
  
 `ppValue`  
 <span data-ttu-id="873ec-117">[out]返回此成员的常量字符串值。</span><span class="sxs-lookup"><span data-stu-id="873ec-117">[out] A constant string value returned by this member.</span></span>  
  
 `pcchValue`  
 <span data-ttu-id="873ec-118">[out]以字符为单位的大小`ppValue`，或为零`ppValue`不包含一个字符串。</span><span class="sxs-lookup"><span data-stu-id="873ec-118">[out] The size in characters of `ppValue`, or zero if `ppValue` does not hold a string.</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="873ec-119">要求</span><span class="sxs-lookup"><span data-stu-id="873ec-119">Requirements</span></span>  
 <span data-ttu-id="873ec-120">**平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。</span><span class="sxs-lookup"><span data-stu-id="873ec-120">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="873ec-121">**标头：** Cor.h</span><span class="sxs-lookup"><span data-stu-id="873ec-121">**Header:** Cor.h</span></span>  
  
 <span data-ttu-id="873ec-122">**库：**作为 MsCorEE.dll 中的资源</span><span class="sxs-lookup"><span data-stu-id="873ec-122">**Library:** Included as a resource in MsCorEE.dll</span></span>  
  
 <span data-ttu-id="873ec-123">**.NET framework 版本：**[!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="873ec-123">**.NET Framework Versions:** [!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="873ec-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="873ec-124">See Also</span></span>  
 [<span data-ttu-id="873ec-125">IMetaDataImport 接口</span><span class="sxs-lookup"><span data-stu-id="873ec-125">IMetaDataImport Interface</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-interface.md)  
 [<span data-ttu-id="873ec-126">IMetaDataImport2 接口</span><span class="sxs-lookup"><span data-stu-id="873ec-126">IMetaDataImport2 Interface</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport2-interface.md)