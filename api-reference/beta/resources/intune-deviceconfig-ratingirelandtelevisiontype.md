---
title: RatingIrelandTelevisionType Enum-Typ
description: TV zum Bewerten Bezeichnungen in Irland
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b357a2604479789cc85c17b0867cb56fa8cc2b3d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991832"
---
# <a name="ratingirelandtelevisiontype-enum-type"></a><span data-ttu-id="d56c3-103">RatingIrelandTelevisionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="d56c3-103">ratingIrelandTelevisionType enum type</span></span>

> <span data-ttu-id="d56c3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d56c3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d56c3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d56c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d56c3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d56c3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d56c3-107">TV zum Bewerten Bezeichnungen in Irland</span><span class="sxs-lookup"><span data-stu-id="d56c3-107">TV content rating labels in Ireland</span></span>
## <a name="members"></a><span data-ttu-id="d56c3-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="d56c3-108">Members</span></span>
|<span data-ttu-id="d56c3-109">Element</span><span class="sxs-lookup"><span data-stu-id="d56c3-109">Member</span></span>|<span data-ttu-id="d56c3-110">Wert</span><span class="sxs-lookup"><span data-stu-id="d56c3-110">Value</span></span>|<span data-ttu-id="d56c3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d56c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d56c3-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="d56c3-112">allAllowed</span></span>|<span data-ttu-id="d56c3-113">0</span><span class="sxs-lookup"><span data-stu-id="d56c3-113">0</span></span>|<span data-ttu-id="d56c3-114">Standardwert, zulassen, dass alle TV Inhalt anzeigt.</span><span class="sxs-lookup"><span data-stu-id="d56c3-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="d56c3-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="d56c3-115">allBlocked</span></span>|<span data-ttu-id="d56c3-116">1</span><span class="sxs-lookup"><span data-stu-id="d56c3-116">1</span></span>|<span data-ttu-id="d56c3-117">Lassen Sie nicht, dass alle TV Inhalt anzeigt.</span><span class="sxs-lookup"><span data-stu-id="d56c3-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="d56c3-118">Allgemeine</span><span class="sxs-lookup"><span data-stu-id="d56c3-118">general</span></span>|<span data-ttu-id="d56c3-119">2</span><span class="sxs-lookup"><span data-stu-id="d56c3-119">2</span></span>|<span data-ttu-id="d56c3-120">Die Klassifizierung GA eignet sich für alle Benutzergruppen</span><span class="sxs-lookup"><span data-stu-id="d56c3-120">The GA classification is suitable for all audiences</span></span>|
|<span data-ttu-id="d56c3-121">Untergeordnetes Element</span><span class="sxs-lookup"><span data-stu-id="d56c3-121">children</span></span>|<span data-ttu-id="d56c3-122">3</span><span class="sxs-lookup"><span data-stu-id="d56c3-122">3</span></span>|<span data-ttu-id="d56c3-123">Die Kapitel Klassifizierung eignet sich für untergeordnete Elemente</span><span class="sxs-lookup"><span data-stu-id="d56c3-123">The CH classification is suitable for children</span></span>|
|<span data-ttu-id="d56c3-124">youngAdults</span><span class="sxs-lookup"><span data-stu-id="d56c3-124">youngAdults</span></span>|<span data-ttu-id="d56c3-125">4</span><span class="sxs-lookup"><span data-stu-id="d56c3-125">4</span></span>|<span data-ttu-id="d56c3-126">Die Klassifizierung YA eignet sich für Teenager</span><span class="sxs-lookup"><span data-stu-id="d56c3-126">The YA classification is suitable for teenage audience</span></span>|
|<span data-ttu-id="d56c3-127">parentalSupervision</span><span class="sxs-lookup"><span data-stu-id="d56c3-127">parentalSupervision</span></span>|<span data-ttu-id="d56c3-128">5</span><span class="sxs-lookup"><span data-stu-id="d56c3-128">5</span></span>|<span data-ttu-id="d56c3-129">PS-Klassifizierung invites Eltern und Aufsichtspersonen, Einschränkung untergeordnete Elemente Access berücksichtigt werden sollten</span><span class="sxs-lookup"><span data-stu-id="d56c3-129">The PS classification invites parents and guardians to consider restriction children’s access</span></span>|
|<span data-ttu-id="d56c3-130">Erfahrungswerte</span><span class="sxs-lookup"><span data-stu-id="d56c3-130">mature</span></span>|<span data-ttu-id="d56c3-131">6</span><span class="sxs-lookup"><span data-stu-id="d56c3-131">6</span></span>|<span data-ttu-id="d56c3-132">Die Klassifizierung MA eignet sich für Erwachsene</span><span class="sxs-lookup"><span data-stu-id="d56c3-132">The MA classification is suitable for adults</span></span>|





