---
title: RatingCanadaTelevisionType Enum-Typ
description: TV zum Bewerten Bezeichnungen in Kanada
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e62339ddac6e6666e17ee5e83aee1f53f4a45fe3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949220"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="ebdc2-103">RatingCanadaTelevisionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="ebdc2-103">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="ebdc2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ebdc2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebdc2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ebdc2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ebdc2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ebdc2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebdc2-107">TV zum Bewerten Bezeichnungen in Kanada</span><span class="sxs-lookup"><span data-stu-id="ebdc2-107">TV content rating labels in Canada</span></span>
## <a name="members"></a><span data-ttu-id="ebdc2-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="ebdc2-108">Members</span></span>
|<span data-ttu-id="ebdc2-109">Element</span><span class="sxs-lookup"><span data-stu-id="ebdc2-109">Member</span></span>|<span data-ttu-id="ebdc2-110">Wert</span><span class="sxs-lookup"><span data-stu-id="ebdc2-110">Value</span></span>|<span data-ttu-id="ebdc2-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ebdc2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebdc2-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="ebdc2-112">allAllowed</span></span>|<span data-ttu-id="ebdc2-113">0</span><span class="sxs-lookup"><span data-stu-id="ebdc2-113">0</span></span>|<span data-ttu-id="ebdc2-114">Standardwert, zulassen, dass alle TV Inhalt anzeigt.</span><span class="sxs-lookup"><span data-stu-id="ebdc2-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="ebdc2-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="ebdc2-115">allBlocked</span></span>|<span data-ttu-id="ebdc2-116">1</span><span class="sxs-lookup"><span data-stu-id="ebdc2-116">1</span></span>|<span data-ttu-id="ebdc2-117">Lassen Sie nicht, dass alle TV Inhalt anzeigt.</span><span class="sxs-lookup"><span data-stu-id="ebdc2-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="ebdc2-118">Untergeordnetes Element</span><span class="sxs-lookup"><span data-stu-id="ebdc2-118">children</span></span>|<span data-ttu-id="ebdc2-119">2</span><span class="sxs-lookup"><span data-stu-id="ebdc2-119">2</span></span>|<span data-ttu-id="ebdc2-120">Die C-Klassifikation eignet sich für untergeordnete Elemente Jahren 2 bis 7 Jahre</span><span class="sxs-lookup"><span data-stu-id="ebdc2-120">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="ebdc2-121">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="ebdc2-121">childrenAbove8</span></span>|<span data-ttu-id="ebdc2-122">3</span><span class="sxs-lookup"><span data-stu-id="ebdc2-122">3</span></span>|<span data-ttu-id="ebdc2-123">Die Klassifizierung C8 eignet sich für die untergeordneten Elemente im Alter von 8 +</span><span class="sxs-lookup"><span data-stu-id="ebdc2-123">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="ebdc2-124">Allgemeine</span><span class="sxs-lookup"><span data-stu-id="ebdc2-124">general</span></span>|<span data-ttu-id="ebdc2-125">4</span><span class="sxs-lookup"><span data-stu-id="ebdc2-125">4</span></span>|<span data-ttu-id="ebdc2-126">Die Klassifizierung G eignet sich für allgemeine Zielgruppen</span><span class="sxs-lookup"><span data-stu-id="ebdc2-126">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="ebdc2-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="ebdc2-127">parentalGuidance</span></span>|<span data-ttu-id="ebdc2-128">5</span><span class="sxs-lookup"><span data-stu-id="ebdc2-128">5</span></span>|<span data-ttu-id="ebdc2-129">Bild Eltern Anleitungen</span><span class="sxs-lookup"><span data-stu-id="ebdc2-129">PG, Parental Guidance</span></span>|
|<span data-ttu-id="ebdc2-130">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="ebdc2-130">agesAbove14</span></span>|<span data-ttu-id="ebdc2-131">6</span><span class="sxs-lookup"><span data-stu-id="ebdc2-131">6</span></span>|<span data-ttu-id="ebdc2-132">Die Klassifizierung 14 + ist für Leser von Berichten Jahren 14 und ältere vorgesehen.</span><span class="sxs-lookup"><span data-stu-id="ebdc2-132">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="ebdc2-133">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="ebdc2-133">agesAbove18</span></span>|<span data-ttu-id="ebdc2-134">7</span><span class="sxs-lookup"><span data-stu-id="ebdc2-134">7</span></span>|<span data-ttu-id="ebdc2-135">Die Klassifizierung 18 + ist für Leser von Berichten Jahren 18 und ältere vorgesehen.</span><span class="sxs-lookup"><span data-stu-id="ebdc2-135">The 18+ classification is intended for viewers ages 18 and older</span></span>|





