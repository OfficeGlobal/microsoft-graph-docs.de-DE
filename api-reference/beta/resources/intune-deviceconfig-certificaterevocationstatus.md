---
title: CertificateRevocationStatus Enum-Typ
description: Status der Zertifikatsperre.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8d24d515f992ed396c3530595240a107852d83e1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868306"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="68529-103">CertificateRevocationStatus Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="68529-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="68529-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="68529-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68529-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="68529-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="68529-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="68529-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68529-107">Status der Zertifikatsperre.</span><span class="sxs-lookup"><span data-stu-id="68529-107">Certificate Revocation Status.</span></span>
## <a name="members"></a><span data-ttu-id="68529-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="68529-108">Members</span></span>
|<span data-ttu-id="68529-109">Element</span><span class="sxs-lookup"><span data-stu-id="68529-109">Member</span></span>|<span data-ttu-id="68529-110">Wert</span><span class="sxs-lookup"><span data-stu-id="68529-110">Value</span></span>|<span data-ttu-id="68529-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68529-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68529-112">n/v</span><span class="sxs-lookup"><span data-stu-id="68529-112">none</span></span>|<span data-ttu-id="68529-113">0</span><span class="sxs-lookup"><span data-stu-id="68529-113">0</span></span>|<span data-ttu-id="68529-114">Nicht gesperrt.</span><span class="sxs-lookup"><span data-stu-id="68529-114">Not revoked.</span></span>|
|<span data-ttu-id="68529-115">Ausstehende</span><span class="sxs-lookup"><span data-stu-id="68529-115">pending</span></span>|<span data-ttu-id="68529-116">1</span><span class="sxs-lookup"><span data-stu-id="68529-116">1</span></span>|<span data-ttu-id="68529-117">OCSP ausstehende.</span><span class="sxs-lookup"><span data-stu-id="68529-117">Revocation pending.</span></span>|
|<span data-ttu-id="68529-118">ausgestellt</span><span class="sxs-lookup"><span data-stu-id="68529-118">issued</span></span>|<span data-ttu-id="68529-119">2</span><span class="sxs-lookup"><span data-stu-id="68529-119">2</span></span>|<span data-ttu-id="68529-120">OCSP-Befehl ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="68529-120">Revocation command issued.</span></span>|
|<span data-ttu-id="68529-121">failed</span><span class="sxs-lookup"><span data-stu-id="68529-121">failed</span></span>|<span data-ttu-id="68529-122">3</span><span class="sxs-lookup"><span data-stu-id="68529-122">3</span></span>|<span data-ttu-id="68529-123">OCSP ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="68529-123">Revocation failed.</span></span>|
|<span data-ttu-id="68529-124">widerrufen</span><span class="sxs-lookup"><span data-stu-id="68529-124">revoked</span></span>|<span data-ttu-id="68529-125">4</span><span class="sxs-lookup"><span data-stu-id="68529-125">4</span></span>|<span data-ttu-id="68529-126">Widerrufen.</span><span class="sxs-lookup"><span data-stu-id="68529-126">Revoked.</span></span>|





