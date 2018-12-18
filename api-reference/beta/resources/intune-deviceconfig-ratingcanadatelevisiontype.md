---
title: RatingCanadaTelevisionType Enum-Typ
description: TV zum Bewerten Bezeichnungen in Kanada
author: tfitzmac
ms.openlocfilehash: fdd587a5a0917aea9a8ec028f30b13d1548e6981
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316947"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="a7592-103">RatingCanadaTelevisionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="a7592-103">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="a7592-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a7592-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7592-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a7592-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7592-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a7592-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7592-107">TV zum Bewerten Bezeichnungen in Kanada</span><span class="sxs-lookup"><span data-stu-id="a7592-107">TV content rating labels in Canada</span></span>
## <a name="members"></a><span data-ttu-id="a7592-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="a7592-108">Members</span></span>
|<span data-ttu-id="a7592-109">Member</span><span class="sxs-lookup"><span data-stu-id="a7592-109">Member</span></span>|<span data-ttu-id="a7592-110">Wert</span><span class="sxs-lookup"><span data-stu-id="a7592-110">Value</span></span>|<span data-ttu-id="a7592-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a7592-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7592-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="a7592-112">allAllowed</span></span>|<span data-ttu-id="a7592-113">0</span><span class="sxs-lookup"><span data-stu-id="a7592-113">0</span></span>|<span data-ttu-id="a7592-114">Standardwert, zulassen, dass alle TV Inhalt anzeigt.</span><span class="sxs-lookup"><span data-stu-id="a7592-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="a7592-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="a7592-115">allBlocked</span></span>|<span data-ttu-id="a7592-116">1</span><span class="sxs-lookup"><span data-stu-id="a7592-116">1</span></span>|<span data-ttu-id="a7592-117">Lassen Sie nicht, dass alle TV Inhalt anzeigt.</span><span class="sxs-lookup"><span data-stu-id="a7592-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="a7592-118">Untergeordnetes Element</span><span class="sxs-lookup"><span data-stu-id="a7592-118">children</span></span>|<span data-ttu-id="a7592-119">2</span><span class="sxs-lookup"><span data-stu-id="a7592-119">2</span></span>|<span data-ttu-id="a7592-120">Die C-Klassifikation eignet sich für untergeordnete Elemente Jahren 2 bis 7 Jahre</span><span class="sxs-lookup"><span data-stu-id="a7592-120">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="a7592-121">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="a7592-121">childrenAbove8</span></span>|<span data-ttu-id="a7592-122">3</span><span class="sxs-lookup"><span data-stu-id="a7592-122">3</span></span>|<span data-ttu-id="a7592-123">Die Klassifizierung C8 eignet sich für die untergeordneten Elemente im Alter von 8 +</span><span class="sxs-lookup"><span data-stu-id="a7592-123">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="a7592-124">Allgemeine</span><span class="sxs-lookup"><span data-stu-id="a7592-124">general</span></span>|<span data-ttu-id="a7592-125">4</span><span class="sxs-lookup"><span data-stu-id="a7592-125">4</span></span>|<span data-ttu-id="a7592-126">Die Klassifizierung G eignet sich für allgemeine Zielgruppen</span><span class="sxs-lookup"><span data-stu-id="a7592-126">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="a7592-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="a7592-127">parentalGuidance</span></span>|<span data-ttu-id="a7592-128">5</span><span class="sxs-lookup"><span data-stu-id="a7592-128">5</span></span>|<span data-ttu-id="a7592-129">Bild Eltern Anleitungen</span><span class="sxs-lookup"><span data-stu-id="a7592-129">PG, Parental Guidance</span></span>|
|<span data-ttu-id="a7592-130">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="a7592-130">agesAbove14</span></span>|<span data-ttu-id="a7592-131">6</span><span class="sxs-lookup"><span data-stu-id="a7592-131">6</span></span>|<span data-ttu-id="a7592-132">Die Klassifizierung 14 + ist für Leser von Berichten Jahren 14 und ältere vorgesehen.</span><span class="sxs-lookup"><span data-stu-id="a7592-132">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="a7592-133">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="a7592-133">agesAbove18</span></span>|<span data-ttu-id="a7592-134">7</span><span class="sxs-lookup"><span data-stu-id="a7592-134">7</span></span>|<span data-ttu-id="a7592-135">Die Klassifizierung 18 + ist für Leser von Berichten Jahren 18 und ältere vorgesehen.</span><span class="sxs-lookup"><span data-stu-id="a7592-135">The 18+ classification is intended for viewers ages 18 and older</span></span>|





