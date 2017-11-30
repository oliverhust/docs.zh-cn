---
title: "IMetaDataImport 接口"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: IMetaDataImport
api_location: mscoree.dll
api_type: COM
f1_keywords: IMetaDataImport
helpviewer_keywords: IMetaDataImport interface [.NET Framework metadata]
ms.assetid: 0adbbd35-5e8d-4fec-8268-dc70a07c5975
topic_type: apiref
caps.latest.revision: "16"
author: mairaw
ms.author: mairaw
manager: wpickett
ms.openlocfilehash: 6c7f1c7e99df61cc0cd33e1697de52a039d412df
ms.sourcegitcommit: 4f3fef493080a43e70e951223894768d36ce430a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2017
---
# <a name="imetadataimport-interface"></a><span data-ttu-id="f67e9-102">IMetaDataImport 接口</span><span class="sxs-lookup"><span data-stu-id="f67e9-102">IMetaDataImport Interface</span></span>
<span data-ttu-id="f67e9-103">提供从可迁移可执行 (PE) 文件或其他源（如类型库或独立的运行时元数据二进制文件）导入和操作现有元数据的方法。</span><span class="sxs-lookup"><span data-stu-id="f67e9-103">Provides methods for importing and manipulating existing metadata from a portable executable (PE) file or other source, such as a type library or a stand-alone, run-time metadata binary.</span></span>  
  
## <a name="methods"></a><span data-ttu-id="f67e9-104">方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-104">Methods</span></span>  
  
|<span data-ttu-id="f67e9-105">方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-105">Method</span></span>|<span data-ttu-id="f67e9-106">描述</span><span class="sxs-lookup"><span data-stu-id="f67e9-106">Description</span></span>|  
|------------|-----------------|  
|[<span data-ttu-id="f67e9-107">CloseEnum 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-107">CloseEnum Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-closeenum-method.md)|<span data-ttu-id="f67e9-108">关闭具有指定句柄的枚举器。</span><span class="sxs-lookup"><span data-stu-id="f67e9-108">Closes the enumerator with the specified handle.</span></span>|  
|[<span data-ttu-id="f67e9-109">CountEnum 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-109">CountEnum Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-countenum-method.md)|<span data-ttu-id="f67e9-110">获取具有指定句柄的枚举器中的元素数。</span><span class="sxs-lookup"><span data-stu-id="f67e9-110">Gets the number of elements in the enumerator with the specified handle.</span></span>|  
|[<span data-ttu-id="f67e9-111">EnumCustomAttributes 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-111">EnumCustomAttributes Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enumcustomattributes-method.md)|<span data-ttu-id="f67e9-112">枚举与指定类型或成员关联的自定义特性定义标记的列表。</span><span class="sxs-lookup"><span data-stu-id="f67e9-112">Enumerates a list of custom attribute-definition tokens associated with the specified type or member.</span></span>|  
|[<span data-ttu-id="f67e9-113">EnumEvents 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-113">EnumEvents Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enumevents-method.md)|<span data-ttu-id="f67e9-114">枚举指定的 TypeDef 标记的事件定义标记。</span><span class="sxs-lookup"><span data-stu-id="f67e9-114">Enumerates event definition tokens for the specified TypeDef token.</span></span>|  
|[<span data-ttu-id="f67e9-115">EnumFields 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-115">EnumFields Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enumfields-method.md)|<span data-ttu-id="f67e9-116">枚举指定的 TypeDef 标记所引用的类型的 FieldDef 标记。</span><span class="sxs-lookup"><span data-stu-id="f67e9-116">Enumerates FieldDef tokens for the type referenced by the specified TypeDef token.</span></span>|  
|[<span data-ttu-id="f67e9-117">EnumFieldsWithName 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-117">EnumFieldsWithName Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enumfieldswithname-method.md)|<span data-ttu-id="f67e9-118">枚举具有指定名称的指定类型的 FieldDef 标记。</span><span class="sxs-lookup"><span data-stu-id="f67e9-118">Enumerates FieldDef tokens of the specified type with the specified name.</span></span>|  
|[<span data-ttu-id="f67e9-119">EnumInterfaceImpls 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-119">EnumInterfaceImpls Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enuminterfaceimpls-method.md)|<span data-ttu-id="f67e9-120">枚举表示接口实现的 MethodDef 标记。</span><span class="sxs-lookup"><span data-stu-id="f67e9-120">Enumerates MethodDef tokens representing interface implementations.</span></span>|  
|[<span data-ttu-id="f67e9-121">EnumMemberRefs 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-121">EnumMemberRefs Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enummemberrefs-method.md)|<span data-ttu-id="f67e9-122">枚举表示指定类型成员的 MemberRef 标记。</span><span class="sxs-lookup"><span data-stu-id="f67e9-122">Enumerates MemberRef tokens representing members of the specified type.</span></span>|  
|[<span data-ttu-id="f67e9-123">EnumMembers 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-123">EnumMembers Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enummembers-method.md)|<span data-ttu-id="f67e9-124">枚举表示指定类型的成员的 MemberDef 标记。</span><span class="sxs-lookup"><span data-stu-id="f67e9-124">Enumerates MemberDef tokens representing members of the specified type.</span></span>|  
|[<span data-ttu-id="f67e9-125">EnumMembersWithName 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-125">EnumMembersWithName Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enummemberswithname-method.md)|<span data-ttu-id="f67e9-126">枚举表示具有指定名称的指定类型的成员的 MemberDef 标记。</span><span class="sxs-lookup"><span data-stu-id="f67e9-126">Enumerates MemberDef tokens representing members of the specified type with the specified name.</span></span>|  
|[<span data-ttu-id="f67e9-127">EnumMethodImpls 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-127">EnumMethodImpls Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enummethodimpls-method.md)|<span data-ttu-id="f67e9-128">枚举表示指定类型的方法的 MethodBody 和 MethodDeclaration 标记。</span><span class="sxs-lookup"><span data-stu-id="f67e9-128">Enumerates MethodBody and MethodDeclaration tokens representing methods of the specified type.</span></span>|  
|[<span data-ttu-id="f67e9-129">EnumMethods 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-129">EnumMethods Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enummethods-method.md)|<span data-ttu-id="f67e9-130">枚举表示指定类型的方法的 MethodDef 标记。</span><span class="sxs-lookup"><span data-stu-id="f67e9-130">Enumerates MethodDef tokens representing methods of the specified type.</span></span>|  
|[<span data-ttu-id="f67e9-131">EnumMethodSemantics 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-131">EnumMethodSemantics Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enummethodsemantics-method.md)|<span data-ttu-id="f67e9-132">枚举与指定方法相关的属性和属性更改事件。</span><span class="sxs-lookup"><span data-stu-id="f67e9-132">Enumerates the properties and the property-change events to which the specified method is related.</span></span>|  
|[<span data-ttu-id="f67e9-133">EnumMethodsWithName 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-133">EnumMethodsWithName Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enummethodswithname-method.md)|<span data-ttu-id="f67e9-134">枚举具有指定名称并且由指定的 TypeDef 标记所引用的类型定义的方法。</span><span class="sxs-lookup"><span data-stu-id="f67e9-134">Enumerates methods that have the specified name and that are defined by the type referenced by the specified TypeDef token.</span></span>|  
|[<span data-ttu-id="f67e9-135">EnumModuleRefs 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-135">EnumModuleRefs Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enummodulerefs-method.md)|<span data-ttu-id="f67e9-136">枚举表示导入的模块的 ModuleRef 标记。</span><span class="sxs-lookup"><span data-stu-id="f67e9-136">Enumerates ModuleRef tokens that represent imported modules.</span></span>|  
|[<span data-ttu-id="f67e9-137">EnumParams 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-137">EnumParams Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enumparams-method.md)|<span data-ttu-id="f67e9-138">枚举 ParamDef 标记，这些标记表示指定的 MethodDef 标记所引用的方法的参数。</span><span class="sxs-lookup"><span data-stu-id="f67e9-138">Enumerates ParamDef tokens representing the parameters of the method referenced by the specified MethodDef token.</span></span>|  
|[<span data-ttu-id="f67e9-139">EnumPermissionSets 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-139">EnumPermissionSets Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enumpermissionsets-method.md)|<span data-ttu-id="f67e9-140">枚举指定的元数据范围内的对象的权限。</span><span class="sxs-lookup"><span data-stu-id="f67e9-140">Enumerates permissions for the objects in a specified metadata scope.</span></span>|  
|[<span data-ttu-id="f67e9-141">EnumProperties 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-141">EnumProperties Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enumproperties-method.md)|<span data-ttu-id="f67e9-142">枚举 PropertyDef 标记，这些标记表示指定的 TypeDef 标记所引用的类型的属性。</span><span class="sxs-lookup"><span data-stu-id="f67e9-142">Enumerates PropertyDef tokens representing the properties of the type referenced by the specified TypeDef token.</span></span>|  
|[<span data-ttu-id="f67e9-143">EnumSignatures 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-143">EnumSignatures Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enumsignatures-method.md)|<span data-ttu-id="f67e9-144">枚举当前范围内表示独立签名的 Signature 标记。</span><span class="sxs-lookup"><span data-stu-id="f67e9-144">Enumerates Signature tokens representing stand-alone signatures in the current scope.</span></span>|  
|[<span data-ttu-id="f67e9-145">EnumTypeDefs 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-145">EnumTypeDefs Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enumtypedefs-method.md)|<span data-ttu-id="f67e9-146">枚举表示当前范围内的所有类型的 TypeDef 标记。</span><span class="sxs-lookup"><span data-stu-id="f67e9-146">Enumerates TypeDef tokens representing all types within the current scope.</span></span>|  
|[<span data-ttu-id="f67e9-147">EnumTypeRefs 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-147">EnumTypeRefs Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enumtyperefs-method.md)|<span data-ttu-id="f67e9-148">枚举当前元数据范围内定义的 TypeRef 标记。</span><span class="sxs-lookup"><span data-stu-id="f67e9-148">Enumerates TypeRef tokens defined in the current metadata scope.</span></span>|  
|[<span data-ttu-id="f67e9-149">EnumTypeSpecs 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-149">EnumTypeSpecs Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enumtypespecs-method.md)|<span data-ttu-id="f67e9-150">枚举当前元数据范围内定义的 TypeSpec 标记。</span><span class="sxs-lookup"><span data-stu-id="f67e9-150">Enumerates TypeSpec tokens defined in the current metadata scope.</span></span>|  
|[<span data-ttu-id="f67e9-151">EnumUnresolvedMethods 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-151">EnumUnresolvedMethods Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enumunresolvedmethods-method.md)|<span data-ttu-id="f67e9-152">枚举表示当前元数据范围内未解析的方法的 MemberDef 标记。</span><span class="sxs-lookup"><span data-stu-id="f67e9-152">Enumerates MemberDef tokens representing the unresolved methods in the current metadata scope.</span></span>|  
|[<span data-ttu-id="f67e9-153">EnumUserStrings 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-153">EnumUserStrings Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-enumuserstrings-method.md)|<span data-ttu-id="f67e9-154">枚举表示当前元数据范围内的硬编码字符串的 String 标记。</span><span class="sxs-lookup"><span data-stu-id="f67e9-154">Enumerates String tokens representing hard-coded strings in the current metadata scope.</span></span>|  
|[<span data-ttu-id="f67e9-155">FindField 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-155">FindField Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-findfield-method.md)|<span data-ttu-id="f67e9-156">获取属于指定类型的成员并具有指定的名称和元数据签名的字段的 FieldDef 标记。</span><span class="sxs-lookup"><span data-stu-id="f67e9-156">Gets the FieldDef token for the field that is a member of the specified type, and has the specified name and metadata signature.</span></span>|  
|[<span data-ttu-id="f67e9-157">FindMember 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-157">FindMember Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-findmember-method.md)|<span data-ttu-id="f67e9-158">获取一个指向成员的 MemberDef 标记的指针，该成员由指定的类型定义，并且具有指定的名称和元数据签名。</span><span class="sxs-lookup"><span data-stu-id="f67e9-158">Gets a pointer to the MemberDef token for the member defined by the specified type with the specified name and metadata signature.</span></span>|  
|[<span data-ttu-id="f67e9-159">FindMemberRef 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-159">FindMemberRef Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-findmemberref-method.md)|<span data-ttu-id="f67e9-160">获取一个指向成员的 MemberRef 标记的指针，该成员由指定的类型定义，并且具有指定的名称和元数据签名。</span><span class="sxs-lookup"><span data-stu-id="f67e9-160">Gets a pointer to the MemberRef token for the member defined by the specified type with the specified name and metadata signature.</span></span>|  
|[<span data-ttu-id="f67e9-161">FindMethod 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-161">FindMethod Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-findmethod-method.md)|<span data-ttu-id="f67e9-162">获取一个指向方法的 MethodDef 标记的指针，该方法由指定的类型定义，并且具有指定的名称和元数据签名。</span><span class="sxs-lookup"><span data-stu-id="f67e9-162">Gets a pointer to the MethodDef token for the method defined by the specified type with the specified name and metadata signature.</span></span>|  
|[<span data-ttu-id="f67e9-163">FindTypeDefByName 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-163">FindTypeDefByName Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-findtypedefbyname-method.md)|<span data-ttu-id="f67e9-164">获取一个指向具有指定名称的类型的 TypeDef 元数据标记的指针。</span><span class="sxs-lookup"><span data-stu-id="f67e9-164">Gets a pointer to the TypeDef metadata token for the type with the specified name.</span></span>|  
|[<span data-ttu-id="f67e9-165">FindTypeRef 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-165">FindTypeRef Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-findtyperef-method.md)|<span data-ttu-id="f67e9-166">获取一个指向 TypeRef 元数据标记的指针，该标记通过指定的名称在指定搜索范围内引用类型。</span><span class="sxs-lookup"><span data-stu-id="f67e9-166">Gets a pointer to the TypeRef metadata token that references the type in the specified search scope with the specified name.</span></span>|  
|[<span data-ttu-id="f67e9-167">GetClassLayout 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-167">GetClassLayout Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getclasslayout-method.md)|<span data-ttu-id="f67e9-168">获取指定的 TypeDef 标记所引用类的布局信息。</span><span class="sxs-lookup"><span data-stu-id="f67e9-168">Gets layout information for the class referenced by the specified TypeDef token.</span></span>|  
|[<span data-ttu-id="f67e9-169">GetCustomAttributeByName 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-169">GetCustomAttributeByName Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getcustomattributebyname-method.md)|<span data-ttu-id="f67e9-170">给定自定义特性的名称时，获取该特性的值。</span><span class="sxs-lookup"><span data-stu-id="f67e9-170">Gets the value of the custom attribute, given its name.</span></span>|  
|[<span data-ttu-id="f67e9-171">GetCustomAttributeProps 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-171">GetCustomAttributeProps Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getcustomattributeprops-method.md)|<span data-ttu-id="f67e9-172">获取给定元数据标记的自定义属性的值。</span><span class="sxs-lookup"><span data-stu-id="f67e9-172">Gets the value of the custom attribute, given its metadata token.</span></span>|  
|[<span data-ttu-id="f67e9-173">GetEventProps 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-173">GetEventProps Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-geteventprops-method.md)|<span data-ttu-id="f67e9-174">对于指定的事件标记表示的事件，获取元数据信息，包括声明类型、委托的添加和删除方法、任何标志及其他关联数据。</span><span class="sxs-lookup"><span data-stu-id="f67e9-174">Gets metadata information (including the declaring type, the add and remove methods for delegates, and any flags and other associated data) for the event represented by the specified event token.</span></span>|  
|[<span data-ttu-id="f67e9-175">GetFieldMarshal 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-175">GetFieldMarshal Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getfieldmarshal-method.md)|<span data-ttu-id="f67e9-176">获取一个指针，该指针指向由指定的字段元数据标记表示的字段的本机非托管类型。</span><span class="sxs-lookup"><span data-stu-id="f67e9-176">Gets a pointer to the native, unmanaged type of the field represented by the specified Field metadata token.</span></span>|  
|[<span data-ttu-id="f67e9-177">GetFieldProps 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-177">GetFieldProps Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getfieldprops-method.md)|<span data-ttu-id="f67e9-178">获取与指定 FieldDef 标记引用的字段关联的元数据。</span><span class="sxs-lookup"><span data-stu-id="f67e9-178">Gets metadata associated with the field referenced by the specified FieldDef token.</span></span>|  
|[<span data-ttu-id="f67e9-179">GetInterfaceImplProps 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-179">GetInterfaceImplProps Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getinterfaceimplprops-method.md)|<span data-ttu-id="f67e9-180">对于实现指定方法的类型和声明该方法的接口，获取一个指向其元数据标记的指针。</span><span class="sxs-lookup"><span data-stu-id="f67e9-180">Gets a pointer to the metadata tokens for the type that implements the specified method and for the interface that declares that method.</span></span>|  
|[<span data-ttu-id="f67e9-181">GetMemberProps 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-181">GetMemberProps Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getmemberprops-method.md)|<span data-ttu-id="f67e9-182">获取指定的元数据标记所引用的类型成员的元数据信息，包括名称、二进制签名和相对虚拟地址。</span><span class="sxs-lookup"><span data-stu-id="f67e9-182">Gets metadata information (including the name, binary signature, and relative virtual address) of the type member referenced by the specified metadata token.</span></span>|  
|[<span data-ttu-id="f67e9-183">GetMemberRefProps 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-183">GetMemberRefProps Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getmemberrefprops-method.md)|<span data-ttu-id="f67e9-184">获取与指定标记引用的成员关联的元数据。</span><span class="sxs-lookup"><span data-stu-id="f67e9-184">Gets metadata associated with the member referenced by the specified token.</span></span>|  
|[<span data-ttu-id="f67e9-185">GetMethodProps 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-185">GetMethodProps Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getmethodprops-method.md)|<span data-ttu-id="f67e9-186">获取与指定的 MethodDef 标记引用的方法关联的元数据。</span><span class="sxs-lookup"><span data-stu-id="f67e9-186">Gets the metadata associated with the method referenced by the specified MethodDef token.</span></span>|  
|[<span data-ttu-id="f67e9-187">GetMethodSemantics 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-187">GetMethodSemantics Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getmethodsemantics-method.md)|<span data-ttu-id="f67e9-188">获取一个指针，该指针指向方法（由指定的 MethodDef 标记引用）与成对属性和事件（由指定的 EventProp 标记引用）之间的关系。</span><span class="sxs-lookup"><span data-stu-id="f67e9-188">Gets a pointer to the relationship between the method referenced by the specified MethodDef token and the paired property and event referenced by the specified EventProp token.</span></span>|  
|[<span data-ttu-id="f67e9-189">GetModuleFromScope 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-189">GetModuleFromScope Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getmodulefromscope-method.md)|<span data-ttu-id="f67e9-190">获取指向当前元数据范围内所引用模块的元数据标记的指针。</span><span class="sxs-lookup"><span data-stu-id="f67e9-190">Gets a pointer to the metadata token for the module referenced in the current metadata scope.</span></span>|  
|[<span data-ttu-id="f67e9-191">GetModuleRefProps 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-191">GetModuleRefProps Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getmodulerefprops-method.md)|<span data-ttu-id="f67e9-192">获取指定元数据标记引用的模块的名称。</span><span class="sxs-lookup"><span data-stu-id="f67e9-192">Gets the name of the module referenced by the specified metadata token.</span></span>|  
|[<span data-ttu-id="f67e9-193">GetNameFromToken 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-193">GetNameFromToken Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getnamefromtoken-method.md)|<span data-ttu-id="f67e9-194">获取指定的元数据标记所引用的对象的 UTF-8 名称。</span><span class="sxs-lookup"><span data-stu-id="f67e9-194">Gets the UTF-8 name of the object referenced by the specified metadata token.</span></span>|  
|[<span data-ttu-id="f67e9-195">GetNativeCallConvFromSig 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-195">GetNativeCallConvFromSig Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getnativecallconvfromsig-method.md)|<span data-ttu-id="f67e9-196">获取指定的签名指针所表示的方法的本机调用约定。</span><span class="sxs-lookup"><span data-stu-id="f67e9-196">Gets the native calling convention for the method that is represented by the specified signature pointer.</span></span>|  
|[<span data-ttu-id="f67e9-197">GetNestedClassProps 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-197">GetNestedClassProps Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getnestedclassprops-method.md)|<span data-ttu-id="f67e9-198">获取指定嵌套类型的封闭父类型的 TypeDef 标记。</span><span class="sxs-lookup"><span data-stu-id="f67e9-198">Gets the TypeDef token for the enclosing parent type of the specified nested type.</span></span>|  
|[<span data-ttu-id="f67e9-199">GetParamForMethodIndex 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-199">GetParamForMethodIndex Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getparamformethodindex-method.md)|<span data-ttu-id="f67e9-200">获取一个指向标记的指针，此标记表示在指定的 MethodDef 标记表示的方法的方法参数序列中位于指定序号位置的参数。</span><span class="sxs-lookup"><span data-stu-id="f67e9-200">Gets a pointer to the token that represents the parameter at the specified ordinal position in the sequence of method parameters for the method represented by the specified MethodDef token.</span></span>|  
|[<span data-ttu-id="f67e9-201">GetParamProps 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-201">GetParamProps Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getparamprops-method.md)|<span data-ttu-id="f67e9-202">获取指定的 ParamDef 标记所引用的参数的元数据值。</span><span class="sxs-lookup"><span data-stu-id="f67e9-202">Gets metadata values for the parameter referenced by the specified ParamDef token.</span></span>|  
|[<span data-ttu-id="f67e9-203">GetPermissionSetProps 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-203">GetPermissionSetProps Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getpermissionsetprops-method.md)|<span data-ttu-id="f67e9-204">获取与指定的 Permission 标记所表示的 System.Security.PermissionSet 关联的元数据。</span><span class="sxs-lookup"><span data-stu-id="f67e9-204">Gets the metadata associated with the System.Security.PermissionSet represented by the specified Permission token.</span></span>|  
|[<span data-ttu-id="f67e9-205">GetPinvokeMap</span><span class="sxs-lookup"><span data-stu-id="f67e9-205">GetPinvokeMap</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getpinvokemap-method.md)|<span data-ttu-id="f67e9-206">获取用于表示 PInvoke 调用的目标程序集的 ModuleRef 标记。</span><span class="sxs-lookup"><span data-stu-id="f67e9-206">Gets a ModuleRef token to represent the target assembly of a PInvoke call.</span></span>|  
|[<span data-ttu-id="f67e9-207">GetPropertyProps 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-207">GetPropertyProps Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getpropertyprops-method.md)|<span data-ttu-id="f67e9-208">获取与指定的标记表示的属性关联的元数据。</span><span class="sxs-lookup"><span data-stu-id="f67e9-208">Gets the metadata associated with the property represented by the specified token.</span></span>|  
|[<span data-ttu-id="f67e9-209">GetRVA 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-209">GetRVA Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getrva-method.md)|<span data-ttu-id="f67e9-210">获取由指定标记表示的代码对象的相对虚拟地址的偏移量。</span><span class="sxs-lookup"><span data-stu-id="f67e9-210">Gets the offset of the relative virtual address of the code object represented by the specified token.</span></span>|  
|[<span data-ttu-id="f67e9-211">GetScopeProps 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-211">GetScopeProps Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getscopeprops-method.md)|<span data-ttu-id="f67e9-212">获取当前元数据范围内的程序集或模块的名称和版本标识符（可选）。</span><span class="sxs-lookup"><span data-stu-id="f67e9-212">Gets the name and optionally the version identifier of the assembly or module in the current metadata scope.</span></span>|  
|[<span data-ttu-id="f67e9-213">GetSigFromToken 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-213">GetSigFromToken Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getsigfromtoken-method.md)|<span data-ttu-id="f67e9-214">获取与指定标记关联的二进制元数据签名。</span><span class="sxs-lookup"><span data-stu-id="f67e9-214">Gets the binary metadata signature associated with the specified token.</span></span>|  
|[<span data-ttu-id="f67e9-215">GetTypeDefProps 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-215">GetTypeDefProps Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-gettypedefprops-method.md)|<span data-ttu-id="f67e9-216">返回指定 TypeDef 标记所表示类型的元数据信息。</span><span class="sxs-lookup"><span data-stu-id="f67e9-216">Returns metadata information for the type represented by the specified TypeDef token.</span></span>|  
|[<span data-ttu-id="f67e9-217">GetTypeRefProps 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-217">GetTypeRefProps Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-gettyperefprops-method.md)|<span data-ttu-id="f67e9-218">获取与指定的 TypeRef 标记所引用的类型关联的元数据。</span><span class="sxs-lookup"><span data-stu-id="f67e9-218">Gets the metadata associated with the type referenced by the specified TypeRef token.</span></span>|  
|[<span data-ttu-id="f67e9-219">GetTypeSpecFromToken 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-219">GetTypeSpecFromToken Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-gettypespecfromtoken-method.md)|<span data-ttu-id="f67e9-220">获取指定标记所表示的类型规范的二进制元数据签名。</span><span class="sxs-lookup"><span data-stu-id="f67e9-220">Gets the binary metadata signature of the type specification represented by the specified token.</span></span>|  
|[<span data-ttu-id="f67e9-221">GetUserString 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-221">GetUserString Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-getuserstring-method.md)|<span data-ttu-id="f67e9-222">获取指定元数据标记所表示的文字字符串。</span><span class="sxs-lookup"><span data-stu-id="f67e9-222">Gets the literal string represented by the specified metadata token.</span></span>|  
|[<span data-ttu-id="f67e9-223">IsGlobal 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-223">IsGlobal Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-isglobal-method.md)|<span data-ttu-id="f67e9-224">获取一个值，该值指示由指定的元数据标记表示的字段、方法或类型是否具有全局范围。</span><span class="sxs-lookup"><span data-stu-id="f67e9-224">Gets a value indicating whether the field, method, or type represented by the specified metadata token has global scope.</span></span>|  
|[<span data-ttu-id="f67e9-225">IsValidToken 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-225">IsValidToken Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-isvalidtoken-method.md)|<span data-ttu-id="f67e9-226">获取指示指定的标记是否包含对代码对象的有效引用的值。</span><span class="sxs-lookup"><span data-stu-id="f67e9-226">Gets a value indicating whether the specified token holds a valid reference to a code object.</span></span>|  
|[<span data-ttu-id="f67e9-227">ResetEnum 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-227">ResetEnum Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-resetenum-method.md)|<span data-ttu-id="f67e9-228">将指定的枚举器重置到指定位置。</span><span class="sxs-lookup"><span data-stu-id="f67e9-228">Resets the specified enumerator to the specified position.</span></span>|  
|[<span data-ttu-id="f67e9-229">ResolveTypeRef 方法</span><span class="sxs-lookup"><span data-stu-id="f67e9-229">ResolveTypeRef Method</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport-resolvetyperef-method.md)|<span data-ttu-id="f67e9-230">获取指定的 TypeRef 标记所引用的类型的类型信息。</span><span class="sxs-lookup"><span data-stu-id="f67e9-230">Gets type information for the type referenced by the specified TypeRef token.</span></span>|  
  
## <a name="remarks"></a><span data-ttu-id="f67e9-231">备注</span><span class="sxs-lookup"><span data-stu-id="f67e9-231">Remarks</span></span>  
 <span data-ttu-id="f67e9-232">`IMetaDataImport` 接口的设计主要供将要导入类型信息（例如，开发工具）或管理已部署组件（例如，解析/激活服务）的工具和服务使用。</span><span class="sxs-lookup"><span data-stu-id="f67e9-232">The design of the `IMetaDataImport` interface is intended primarily to be used by tools and services that will be importing type information (for example, development tools) or managing deployed components (for example, resolution/activation services).</span></span> <span data-ttu-id="f67e9-233">`IMetaDataImport` 中的方法属于下列任务类别：</span><span class="sxs-lookup"><span data-stu-id="f67e9-233">The methods in `IMetaDataImport` fall into the following task categories:</span></span>  
  
-   <span data-ttu-id="f67e9-234">枚举元数据范围内的项集合。</span><span class="sxs-lookup"><span data-stu-id="f67e9-234">Enumerating collections of items in the metadata scope.</span></span>  
  
-   <span data-ttu-id="f67e9-235">查找具有特定特征集的项。</span><span class="sxs-lookup"><span data-stu-id="f67e9-235">Finding an item that has a specific set of characteristics.</span></span>  
  
-   <span data-ttu-id="f67e9-236">获取指定项的属性。</span><span class="sxs-lookup"><span data-stu-id="f67e9-236">Getting properties of a specified item.</span></span>  
  
-   <span data-ttu-id="f67e9-237">Get 方法专门用来返回元数据项的单值属性。</span><span class="sxs-lookup"><span data-stu-id="f67e9-237">The Get methods are specifically designed to return single-valued properties of a metadata item.</span></span> <span data-ttu-id="f67e9-238">当该属性是对另一个项的引用时，将返回该项的标记。</span><span class="sxs-lookup"><span data-stu-id="f67e9-238">When the property is a reference to another item, a token for that item is returned.</span></span> <span data-ttu-id="f67e9-239">任何指针输入类型都可为 NULL，以指示未请求特定值。</span><span class="sxs-lookup"><span data-stu-id="f67e9-239">Any pointer input type can be NULL to indicate that the particular value is not being requested.</span></span> <span data-ttu-id="f67e9-240">若要获取基本上由集合对象（例如，某个类实现的接口集合）构成的属性，请使用枚举方法。</span><span class="sxs-lookup"><span data-stu-id="f67e9-240">To obtain properties that are essentially collection objects (for example, the collection of interfaces that a class implements), use the enumeration methods.</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="f67e9-241">要求</span><span class="sxs-lookup"><span data-stu-id="f67e9-241">Requirements</span></span>  
 <span data-ttu-id="f67e9-242">**平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。</span><span class="sxs-lookup"><span data-stu-id="f67e9-242">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="f67e9-243">**标头：** Cor.h</span><span class="sxs-lookup"><span data-stu-id="f67e9-243">**Header:** Cor.h</span></span>  
  
 <span data-ttu-id="f67e9-244">**库：**用作 MsCorEE.dll 中的资源</span><span class="sxs-lookup"><span data-stu-id="f67e9-244">**Library:** Used as a resource in MsCorEE.dll</span></span>  
  
 <span data-ttu-id="f67e9-245">**.NET framework 版本：**[!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="f67e9-245">**.NET Framework Versions:** [!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="f67e9-246">另请参阅</span><span class="sxs-lookup"><span data-stu-id="f67e9-246">See Also</span></span>  
 [<span data-ttu-id="f67e9-247">元数据接口</span><span class="sxs-lookup"><span data-stu-id="f67e9-247">Metadata Interfaces</span></span>](../../../../docs/framework/unmanaged-api/metadata/metadata-interfaces.md)  
 [<span data-ttu-id="f67e9-248">IMetaDataImport2 接口</span><span class="sxs-lookup"><span data-stu-id="f67e9-248">IMetaDataImport2 Interface</span></span>](../../../../docs/framework/unmanaged-api/metadata/imetadataimport2-interface.md)