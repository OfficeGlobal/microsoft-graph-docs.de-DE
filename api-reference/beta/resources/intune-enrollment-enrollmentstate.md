---
title: EnrollmentState Enum-Typ
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 94a3790733067598442af615cb90b8ae347fd228
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869020"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="cba33-103">EnrollmentState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="cba33-103">enrollmentState enum type</span></span>

> <span data-ttu-id="cba33-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cba33-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cba33-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cba33-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cba33-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cba33-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cba33-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="cba33-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="cba33-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="cba33-108">Members</span></span>
|<span data-ttu-id="cba33-109">Element</span><span class="sxs-lookup"><span data-stu-id="cba33-109">Member</span></span>|<span data-ttu-id="cba33-110">Wert</span><span class="sxs-lookup"><span data-stu-id="cba33-110">Value</span></span>|<span data-ttu-id="cba33-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cba33-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cba33-112">unknown</span><span class="sxs-lookup"><span data-stu-id="cba33-112">unknown</span></span>|<span data-ttu-id="cba33-113">0</span><span class="sxs-lookup"><span data-stu-id="cba33-113">0</span></span>|<span data-ttu-id="cba33-114">Die Registrierung des Geräts ist unbekannt</span><span class="sxs-lookup"><span data-stu-id="cba33-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="cba33-115">registriert</span><span class="sxs-lookup"><span data-stu-id="cba33-115">enrolled</span></span>|<span data-ttu-id="cba33-116">1</span><span class="sxs-lookup"><span data-stu-id="cba33-116">1</span></span>|<span data-ttu-id="cba33-117">Gerät ist registriert.</span><span class="sxs-lookup"><span data-stu-id="cba33-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="cba33-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="cba33-118">pendingReset</span></span>|<span data-ttu-id="cba33-119">2</span><span class="sxs-lookup"><span data-stu-id="cba33-119">2</span></span>|<span data-ttu-id="cba33-120">Registriert, aber es über Registrierung Profil registriert ist und das registrierte Profil unterscheidet sich von der zugewiesenen Profil.</span><span class="sxs-lookup"><span data-stu-id="cba33-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="cba33-121">failed</span><span class="sxs-lookup"><span data-stu-id="cba33-121">failed</span></span>|<span data-ttu-id="cba33-122">3</span><span class="sxs-lookup"><span data-stu-id="cba33-122">3</span></span>|<span data-ttu-id="cba33-123">Nicht registriert und Registrierung Fehler Datensatz vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="cba33-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="cba33-124">notContacted</span><span class="sxs-lookup"><span data-stu-id="cba33-124">notContacted</span></span>|<span data-ttu-id="cba33-125">4</span><span class="sxs-lookup"><span data-stu-id="cba33-125">4</span></span>|<span data-ttu-id="cba33-126">Gerät ist importiert, aber nicht registriert.</span><span class="sxs-lookup"><span data-stu-id="cba33-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="cba33-127">gesperrt</span><span class="sxs-lookup"><span data-stu-id="cba33-127">blocked</span></span>|<span data-ttu-id="cba33-128">5</span><span class="sxs-lookup"><span data-stu-id="cba33-128">5</span></span>|<span data-ttu-id="cba33-129">Gerät als userless registriert ist, aber wird blockiert zu Benutzer Registrierung navigieren, da die app konnte nicht installiert werden.</span><span class="sxs-lookup"><span data-stu-id="cba33-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|





