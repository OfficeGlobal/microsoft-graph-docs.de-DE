---
title: DeviceManagementPartnerAppType Enum-Typ
description: Partner-App-Typ.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6abfc248208cb3b9384eef3ed0772be61a77539c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922123"
---
# <a name="devicemanagementpartnerapptype-enum-type"></a><span data-ttu-id="c823c-103">DeviceManagementPartnerAppType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="c823c-103">deviceManagementPartnerAppType enum type</span></span>

> <span data-ttu-id="c823c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c823c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c823c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c823c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c823c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c823c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c823c-107">Partner-App-Typ.</span><span class="sxs-lookup"><span data-stu-id="c823c-107">Partner App Type.</span></span>
## <a name="members"></a><span data-ttu-id="c823c-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="c823c-108">Members</span></span>
|<span data-ttu-id="c823c-109">Element</span><span class="sxs-lookup"><span data-stu-id="c823c-109">Member</span></span>|<span data-ttu-id="c823c-110">Wert</span><span class="sxs-lookup"><span data-stu-id="c823c-110">Value</span></span>|<span data-ttu-id="c823c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c823c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c823c-112">unknown</span><span class="sxs-lookup"><span data-stu-id="c823c-112">unknown</span></span>|<span data-ttu-id="c823c-113">0</span><span class="sxs-lookup"><span data-stu-id="c823c-113">0</span></span>|<span data-ttu-id="c823c-114">Partner-App-Typ ist unbekannt.</span><span class="sxs-lookup"><span data-stu-id="c823c-114">Partner App type is unknown.</span></span>|
|<span data-ttu-id="c823c-115">singleTenantApp</span><span class="sxs-lookup"><span data-stu-id="c823c-115">singleTenantApp</span></span>|<span data-ttu-id="c823c-116">1</span><span class="sxs-lookup"><span data-stu-id="c823c-116">1</span></span>|<span data-ttu-id="c823c-117">Partner App ist mit einem einzelnen Mandanten in AAD.</span><span class="sxs-lookup"><span data-stu-id="c823c-117">Partner App is Single tenant in AAD.</span></span>|
|<span data-ttu-id="c823c-118">multiTenantApp</span><span class="sxs-lookup"><span data-stu-id="c823c-118">multiTenantApp</span></span>|<span data-ttu-id="c823c-119">2</span><span class="sxs-lookup"><span data-stu-id="c823c-119">2</span></span>|<span data-ttu-id="c823c-120">Partner App ist mit mehreren Mandanten in AAD.</span><span class="sxs-lookup"><span data-stu-id="c823c-120">Partner App is Multi tenant in AAD.</span></span>|





