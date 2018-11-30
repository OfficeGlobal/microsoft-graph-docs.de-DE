---
title: CertificateRevocationStatus Enum-Typ
description: Status der Zertifikatsperre.
ms.openlocfilehash: 5fb80b85cb6fe65e20439f8a3242b6bc74b30184
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059606"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="cbe15-103">CertificateRevocationStatus Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="cbe15-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="cbe15-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cbe15-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cbe15-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cbe15-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cbe15-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cbe15-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cbe15-107">Status der Zertifikatsperre.</span><span class="sxs-lookup"><span data-stu-id="cbe15-107">Certificate Revocation Status.</span></span>
## <a name="members"></a><span data-ttu-id="cbe15-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="cbe15-108">Members</span></span>
|<span data-ttu-id="cbe15-109">Element</span><span class="sxs-lookup"><span data-stu-id="cbe15-109">Member</span></span>|<span data-ttu-id="cbe15-110">Wert</span><span class="sxs-lookup"><span data-stu-id="cbe15-110">Value</span></span>|<span data-ttu-id="cbe15-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cbe15-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbe15-112">n/v</span><span class="sxs-lookup"><span data-stu-id="cbe15-112">none</span></span>|<span data-ttu-id="cbe15-113">0</span><span class="sxs-lookup"><span data-stu-id="cbe15-113">0</span></span>|<span data-ttu-id="cbe15-114">Nicht gesperrt.</span><span class="sxs-lookup"><span data-stu-id="cbe15-114">Not revoked.</span></span>|
|<span data-ttu-id="cbe15-115">Ausstehende</span><span class="sxs-lookup"><span data-stu-id="cbe15-115">pending</span></span>|<span data-ttu-id="cbe15-116">1</span><span class="sxs-lookup"><span data-stu-id="cbe15-116">1</span></span>|<span data-ttu-id="cbe15-117">OCSP ausstehende.</span><span class="sxs-lookup"><span data-stu-id="cbe15-117">Revocation pending.</span></span>|
|<span data-ttu-id="cbe15-118">ausgestellt</span><span class="sxs-lookup"><span data-stu-id="cbe15-118">issued</span></span>|<span data-ttu-id="cbe15-119">2</span><span class="sxs-lookup"><span data-stu-id="cbe15-119">2</span></span>|<span data-ttu-id="cbe15-120">OCSP-Befehl ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="cbe15-120">Revocation command issued.</span></span>|
|<span data-ttu-id="cbe15-121">failed</span><span class="sxs-lookup"><span data-stu-id="cbe15-121">failed</span></span>|<span data-ttu-id="cbe15-122">3</span><span class="sxs-lookup"><span data-stu-id="cbe15-122">3</span></span>|<span data-ttu-id="cbe15-123">OCSP ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="cbe15-123">Revocation failed.</span></span>|
|<span data-ttu-id="cbe15-124">widerrufen</span><span class="sxs-lookup"><span data-stu-id="cbe15-124">revoked</span></span>|<span data-ttu-id="cbe15-125">4</span><span class="sxs-lookup"><span data-stu-id="cbe15-125">4</span></span>|<span data-ttu-id="cbe15-126">Widerrufen.</span><span class="sxs-lookup"><span data-stu-id="cbe15-126">Revoked.</span></span>|





