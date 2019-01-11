---
title: RatingIrelandTelevisionType Enum-Typ
description: TV zum Bewerten Bezeichnungen in Irland
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 37485c407a5261bbf23434ad524f95b28e8f1e48
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860984"
---
# <a name="ratingirelandtelevisiontype-enum-type"></a><span data-ttu-id="b64d6-103">RatingIrelandTelevisionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="b64d6-103">ratingIrelandTelevisionType enum type</span></span>

> <span data-ttu-id="b64d6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b64d6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b64d6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b64d6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b64d6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b64d6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b64d6-107">TV zum Bewerten Bezeichnungen in Irland</span><span class="sxs-lookup"><span data-stu-id="b64d6-107">TV content rating labels in Ireland</span></span>
## <a name="members"></a><span data-ttu-id="b64d6-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="b64d6-108">Members</span></span>
|<span data-ttu-id="b64d6-109">Element</span><span class="sxs-lookup"><span data-stu-id="b64d6-109">Member</span></span>|<span data-ttu-id="b64d6-110">Wert</span><span class="sxs-lookup"><span data-stu-id="b64d6-110">Value</span></span>|<span data-ttu-id="b64d6-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b64d6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b64d6-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="b64d6-112">allAllowed</span></span>|<span data-ttu-id="b64d6-113">0</span><span class="sxs-lookup"><span data-stu-id="b64d6-113">0</span></span>|<span data-ttu-id="b64d6-114">Standardwert, zulassen, dass alle TV Inhalt anzeigt.</span><span class="sxs-lookup"><span data-stu-id="b64d6-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="b64d6-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="b64d6-115">allBlocked</span></span>|<span data-ttu-id="b64d6-116">1</span><span class="sxs-lookup"><span data-stu-id="b64d6-116">1</span></span>|<span data-ttu-id="b64d6-117">Lassen Sie nicht, dass alle TV Inhalt anzeigt.</span><span class="sxs-lookup"><span data-stu-id="b64d6-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="b64d6-118">Allgemeine</span><span class="sxs-lookup"><span data-stu-id="b64d6-118">general</span></span>|<span data-ttu-id="b64d6-119">2</span><span class="sxs-lookup"><span data-stu-id="b64d6-119">2</span></span>|<span data-ttu-id="b64d6-120">Die Klassifizierung GA eignet sich für alle Benutzergruppen</span><span class="sxs-lookup"><span data-stu-id="b64d6-120">The GA classification is suitable for all audiences</span></span>|
|<span data-ttu-id="b64d6-121">Untergeordnetes Element</span><span class="sxs-lookup"><span data-stu-id="b64d6-121">children</span></span>|<span data-ttu-id="b64d6-122">3</span><span class="sxs-lookup"><span data-stu-id="b64d6-122">3</span></span>|<span data-ttu-id="b64d6-123">Die Kapitel Klassifizierung eignet sich für untergeordnete Elemente</span><span class="sxs-lookup"><span data-stu-id="b64d6-123">The CH classification is suitable for children</span></span>|
|<span data-ttu-id="b64d6-124">youngAdults</span><span class="sxs-lookup"><span data-stu-id="b64d6-124">youngAdults</span></span>|<span data-ttu-id="b64d6-125">4</span><span class="sxs-lookup"><span data-stu-id="b64d6-125">4</span></span>|<span data-ttu-id="b64d6-126">Die Klassifizierung YA eignet sich für Teenager</span><span class="sxs-lookup"><span data-stu-id="b64d6-126">The YA classification is suitable for teenage audience</span></span>|
|<span data-ttu-id="b64d6-127">parentalSupervision</span><span class="sxs-lookup"><span data-stu-id="b64d6-127">parentalSupervision</span></span>|<span data-ttu-id="b64d6-128">5</span><span class="sxs-lookup"><span data-stu-id="b64d6-128">5</span></span>|<span data-ttu-id="b64d6-129">PS-Klassifizierung invites Eltern und Aufsichtspersonen, Einschränkung untergeordnete Elemente Access berücksichtigt werden sollten</span><span class="sxs-lookup"><span data-stu-id="b64d6-129">The PS classification invites parents and guardians to consider restriction children’s access</span></span>|
|<span data-ttu-id="b64d6-130">Erfahrungswerte</span><span class="sxs-lookup"><span data-stu-id="b64d6-130">mature</span></span>|<span data-ttu-id="b64d6-131">6</span><span class="sxs-lookup"><span data-stu-id="b64d6-131">6</span></span>|<span data-ttu-id="b64d6-132">Die Klassifizierung MA eignet sich für Erwachsene</span><span class="sxs-lookup"><span data-stu-id="b64d6-132">The MA classification is suitable for adults</span></span>|





