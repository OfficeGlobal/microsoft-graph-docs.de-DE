---
title: EmailSyncDuration Enum-Typ
description: Mögliche Werte für die Dauer der e-Mail-Synchronisierung.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fcabbe69c10cd490732560ea856c39c5cfd8cb44
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986411"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="df5fe-103">EmailSyncDuration Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="df5fe-103">emailSyncDuration enum type</span></span>

> <span data-ttu-id="df5fe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="df5fe-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df5fe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df5fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df5fe-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="df5fe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df5fe-107">Mögliche Werte für die Dauer der e-Mail-Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="df5fe-107">Possible values for email sync duration.</span></span>
## <a name="members"></a><span data-ttu-id="df5fe-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="df5fe-108">Members</span></span>
|<span data-ttu-id="df5fe-109">Element</span><span class="sxs-lookup"><span data-stu-id="df5fe-109">Member</span></span>|<span data-ttu-id="df5fe-110">Wert</span><span class="sxs-lookup"><span data-stu-id="df5fe-110">Value</span></span>|<span data-ttu-id="df5fe-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df5fe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df5fe-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="df5fe-112">userDefined</span></span>|<span data-ttu-id="df5fe-113">0</span><span class="sxs-lookup"><span data-stu-id="df5fe-113">0</span></span>|<span data-ttu-id="df5fe-114">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="df5fe-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="df5fe-115">oneDay</span><span class="sxs-lookup"><span data-stu-id="df5fe-115">oneDay</span></span>|<span data-ttu-id="df5fe-116">1</span><span class="sxs-lookup"><span data-stu-id="df5fe-116">1</span></span>|<span data-ttu-id="df5fe-117">Synchronisieren von e-Mail für einen Tag.</span><span class="sxs-lookup"><span data-stu-id="df5fe-117">Sync one day of email.</span></span>|
|<span data-ttu-id="df5fe-118">threeDays</span><span class="sxs-lookup"><span data-stu-id="df5fe-118">threeDays</span></span>|<span data-ttu-id="df5fe-119">2</span><span class="sxs-lookup"><span data-stu-id="df5fe-119">2</span></span>|<span data-ttu-id="df5fe-120">Synchronisieren Sie drei Tage von e-Mails.</span><span class="sxs-lookup"><span data-stu-id="df5fe-120">Sync three days of email.</span></span>|
|<span data-ttu-id="df5fe-121">oneWeek</span><span class="sxs-lookup"><span data-stu-id="df5fe-121">oneWeek</span></span>|<span data-ttu-id="df5fe-122">3</span><span class="sxs-lookup"><span data-stu-id="df5fe-122">3</span></span>|<span data-ttu-id="df5fe-123">Synchronisieren Sie eine Woche vor e-Mail.</span><span class="sxs-lookup"><span data-stu-id="df5fe-123">Sync one week of email.</span></span>|
|<span data-ttu-id="df5fe-124">twoWeeks</span><span class="sxs-lookup"><span data-stu-id="df5fe-124">twoWeeks</span></span>|<span data-ttu-id="df5fe-125">4</span><span class="sxs-lookup"><span data-stu-id="df5fe-125">4</span></span>|<span data-ttu-id="df5fe-126">Synchronisieren von zwei Wochen von e-Mails.</span><span class="sxs-lookup"><span data-stu-id="df5fe-126">Sync two weeks of email.</span></span>|
|<span data-ttu-id="df5fe-127">oneMonth</span><span class="sxs-lookup"><span data-stu-id="df5fe-127">oneMonth</span></span>|<span data-ttu-id="df5fe-128">5</span><span class="sxs-lookup"><span data-stu-id="df5fe-128">5</span></span>|<span data-ttu-id="df5fe-129">Synchronisieren eines Monats e-Mail.</span><span class="sxs-lookup"><span data-stu-id="df5fe-129">Sync one month of email.</span></span>|
|<span data-ttu-id="df5fe-130">unbegrenzt</span><span class="sxs-lookup"><span data-stu-id="df5fe-130">unlimited</span></span>|<span data-ttu-id="df5fe-131">6</span><span class="sxs-lookup"><span data-stu-id="df5fe-131">6</span></span>|<span data-ttu-id="df5fe-132">Synchronisieren Sie eine unbegrenzte Dauer von e-Mail.</span><span class="sxs-lookup"><span data-stu-id="df5fe-132">Sync an unlimited duration of email.</span></span>|





