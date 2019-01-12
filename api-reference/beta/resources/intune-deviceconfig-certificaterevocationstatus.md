---
title: CertificateRevocationStatus Enum-Typ
description: Status der Zertifikatsperre.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8c1c77e267da5528088a7a8ef6400a872790aaf3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983121"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="0ceb1-103">CertificateRevocationStatus Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="0ceb1-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="0ceb1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0ceb1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ceb1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0ceb1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ceb1-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0ceb1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ceb1-107">Status der Zertifikatsperre.</span><span class="sxs-lookup"><span data-stu-id="0ceb1-107">Certificate Revocation Status.</span></span>
## <a name="members"></a><span data-ttu-id="0ceb1-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="0ceb1-108">Members</span></span>
|<span data-ttu-id="0ceb1-109">Element</span><span class="sxs-lookup"><span data-stu-id="0ceb1-109">Member</span></span>|<span data-ttu-id="0ceb1-110">Wert</span><span class="sxs-lookup"><span data-stu-id="0ceb1-110">Value</span></span>|<span data-ttu-id="0ceb1-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0ceb1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ceb1-112">n/v</span><span class="sxs-lookup"><span data-stu-id="0ceb1-112">none</span></span>|<span data-ttu-id="0ceb1-113">0</span><span class="sxs-lookup"><span data-stu-id="0ceb1-113">0</span></span>|<span data-ttu-id="0ceb1-114">Nicht gesperrt.</span><span class="sxs-lookup"><span data-stu-id="0ceb1-114">Not revoked.</span></span>|
|<span data-ttu-id="0ceb1-115">Ausstehende</span><span class="sxs-lookup"><span data-stu-id="0ceb1-115">pending</span></span>|<span data-ttu-id="0ceb1-116">1</span><span class="sxs-lookup"><span data-stu-id="0ceb1-116">1</span></span>|<span data-ttu-id="0ceb1-117">OCSP ausstehende.</span><span class="sxs-lookup"><span data-stu-id="0ceb1-117">Revocation pending.</span></span>|
|<span data-ttu-id="0ceb1-118">ausgestellt</span><span class="sxs-lookup"><span data-stu-id="0ceb1-118">issued</span></span>|<span data-ttu-id="0ceb1-119">2</span><span class="sxs-lookup"><span data-stu-id="0ceb1-119">2</span></span>|<span data-ttu-id="0ceb1-120">OCSP-Befehl ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="0ceb1-120">Revocation command issued.</span></span>|
|<span data-ttu-id="0ceb1-121">failed</span><span class="sxs-lookup"><span data-stu-id="0ceb1-121">failed</span></span>|<span data-ttu-id="0ceb1-122">3</span><span class="sxs-lookup"><span data-stu-id="0ceb1-122">3</span></span>|<span data-ttu-id="0ceb1-123">OCSP ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="0ceb1-123">Revocation failed.</span></span>|
|<span data-ttu-id="0ceb1-124">widerrufen</span><span class="sxs-lookup"><span data-stu-id="0ceb1-124">revoked</span></span>|<span data-ttu-id="0ceb1-125">4</span><span class="sxs-lookup"><span data-stu-id="0ceb1-125">4</span></span>|<span data-ttu-id="0ceb1-126">Widerrufen.</span><span class="sxs-lookup"><span data-stu-id="0ceb1-126">Revoked.</span></span>|





