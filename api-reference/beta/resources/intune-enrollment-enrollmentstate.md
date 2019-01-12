---
title: EnrollmentState Enum-Typ
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9394755c5b6e6de8ed039b226d03074f1ef16cc3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933589"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="5896f-103">EnrollmentState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="5896f-103">enrollmentState enum type</span></span>

> <span data-ttu-id="5896f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5896f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5896f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5896f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5896f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5896f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5896f-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="5896f-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="5896f-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="5896f-108">Members</span></span>
|<span data-ttu-id="5896f-109">Element</span><span class="sxs-lookup"><span data-stu-id="5896f-109">Member</span></span>|<span data-ttu-id="5896f-110">Wert</span><span class="sxs-lookup"><span data-stu-id="5896f-110">Value</span></span>|<span data-ttu-id="5896f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5896f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5896f-112">unknown</span><span class="sxs-lookup"><span data-stu-id="5896f-112">unknown</span></span>|<span data-ttu-id="5896f-113">0</span><span class="sxs-lookup"><span data-stu-id="5896f-113">0</span></span>|<span data-ttu-id="5896f-114">Die Registrierung des Geräts ist unbekannt</span><span class="sxs-lookup"><span data-stu-id="5896f-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="5896f-115">registriert</span><span class="sxs-lookup"><span data-stu-id="5896f-115">enrolled</span></span>|<span data-ttu-id="5896f-116">1</span><span class="sxs-lookup"><span data-stu-id="5896f-116">1</span></span>|<span data-ttu-id="5896f-117">Gerät ist registriert.</span><span class="sxs-lookup"><span data-stu-id="5896f-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="5896f-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="5896f-118">pendingReset</span></span>|<span data-ttu-id="5896f-119">2</span><span class="sxs-lookup"><span data-stu-id="5896f-119">2</span></span>|<span data-ttu-id="5896f-120">Registriert, aber es über Registrierung Profil registriert ist und das registrierte Profil unterscheidet sich von der zugewiesenen Profil.</span><span class="sxs-lookup"><span data-stu-id="5896f-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="5896f-121">failed</span><span class="sxs-lookup"><span data-stu-id="5896f-121">failed</span></span>|<span data-ttu-id="5896f-122">3</span><span class="sxs-lookup"><span data-stu-id="5896f-122">3</span></span>|<span data-ttu-id="5896f-123">Nicht registriert und Registrierung Fehler Datensatz vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="5896f-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="5896f-124">notContacted</span><span class="sxs-lookup"><span data-stu-id="5896f-124">notContacted</span></span>|<span data-ttu-id="5896f-125">4</span><span class="sxs-lookup"><span data-stu-id="5896f-125">4</span></span>|<span data-ttu-id="5896f-126">Gerät ist importiert, aber nicht registriert.</span><span class="sxs-lookup"><span data-stu-id="5896f-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="5896f-127">gesperrt</span><span class="sxs-lookup"><span data-stu-id="5896f-127">blocked</span></span>|<span data-ttu-id="5896f-128">5</span><span class="sxs-lookup"><span data-stu-id="5896f-128">5</span></span>|<span data-ttu-id="5896f-129">Gerät als userless registriert ist, aber wird blockiert zu Benutzer Registrierung navigieren, da die app konnte nicht installiert werden.</span><span class="sxs-lookup"><span data-stu-id="5896f-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|





