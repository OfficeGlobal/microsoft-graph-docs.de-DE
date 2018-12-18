---
title: CertificateRevocationStatus Enum-Typ
description: Status der Zertifikatsperre.
author: tfitzmac
ms.openlocfilehash: d41845ba882136c15d944c8a7f91083e6fa47cdb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358226"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="f55f7-103">CertificateRevocationStatus Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="f55f7-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="f55f7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f55f7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f55f7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f55f7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f55f7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f55f7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f55f7-107">Status der Zertifikatsperre.</span><span class="sxs-lookup"><span data-stu-id="f55f7-107">Certificate Revocation Status.</span></span>
## <a name="members"></a><span data-ttu-id="f55f7-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="f55f7-108">Members</span></span>
|<span data-ttu-id="f55f7-109">Member</span><span class="sxs-lookup"><span data-stu-id="f55f7-109">Member</span></span>|<span data-ttu-id="f55f7-110">Wert</span><span class="sxs-lookup"><span data-stu-id="f55f7-110">Value</span></span>|<span data-ttu-id="f55f7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f55f7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f55f7-112">Keine</span><span class="sxs-lookup"><span data-stu-id="f55f7-112">none</span></span>|<span data-ttu-id="f55f7-113">0</span><span class="sxs-lookup"><span data-stu-id="f55f7-113">0</span></span>|<span data-ttu-id="f55f7-114">Nicht gesperrt.</span><span class="sxs-lookup"><span data-stu-id="f55f7-114">Not revoked.</span></span>|
|<span data-ttu-id="f55f7-115">Ausstehende</span><span class="sxs-lookup"><span data-stu-id="f55f7-115">pending</span></span>|<span data-ttu-id="f55f7-116">1</span><span class="sxs-lookup"><span data-stu-id="f55f7-116">1</span></span>|<span data-ttu-id="f55f7-117">OCSP ausstehende.</span><span class="sxs-lookup"><span data-stu-id="f55f7-117">Revocation pending.</span></span>|
|<span data-ttu-id="f55f7-118">ausgestellt</span><span class="sxs-lookup"><span data-stu-id="f55f7-118">issued</span></span>|<span data-ttu-id="f55f7-119">2</span><span class="sxs-lookup"><span data-stu-id="f55f7-119">2</span></span>|<span data-ttu-id="f55f7-120">OCSP-Befehl ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="f55f7-120">Revocation command issued.</span></span>|
|<span data-ttu-id="f55f7-121">failed</span><span class="sxs-lookup"><span data-stu-id="f55f7-121">failed</span></span>|<span data-ttu-id="f55f7-122">3</span><span class="sxs-lookup"><span data-stu-id="f55f7-122">3</span></span>|<span data-ttu-id="f55f7-123">OCSP ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="f55f7-123">Revocation failed.</span></span>|
|<span data-ttu-id="f55f7-124">widerrufen</span><span class="sxs-lookup"><span data-stu-id="f55f7-124">revoked</span></span>|<span data-ttu-id="f55f7-125">4</span><span class="sxs-lookup"><span data-stu-id="f55f7-125">4</span></span>|<span data-ttu-id="f55f7-126">Widerrufen.</span><span class="sxs-lookup"><span data-stu-id="f55f7-126">Revoked.</span></span>|





