---
title: EnrollmentState Enum-Typ
description: Noch nicht dokumentiert
ms.openlocfilehash: 8e8e20c0fd04e4da57eddfa7384052a6ab468152
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064084"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="f4cd0-103">EnrollmentState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="f4cd0-103">enrollmentState enum type</span></span>

> <span data-ttu-id="f4cd0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f4cd0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f4cd0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f4cd0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4cd0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f4cd0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4cd0-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f4cd0-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="f4cd0-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="f4cd0-108">Members</span></span>
|<span data-ttu-id="f4cd0-109">Element</span><span class="sxs-lookup"><span data-stu-id="f4cd0-109">Member</span></span>|<span data-ttu-id="f4cd0-110">Wert</span><span class="sxs-lookup"><span data-stu-id="f4cd0-110">Value</span></span>|<span data-ttu-id="f4cd0-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4cd0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4cd0-112">unknown</span><span class="sxs-lookup"><span data-stu-id="f4cd0-112">unknown</span></span>|<span data-ttu-id="f4cd0-113">0</span><span class="sxs-lookup"><span data-stu-id="f4cd0-113">0</span></span>|<span data-ttu-id="f4cd0-114">Die Registrierung des Geräts ist unbekannt</span><span class="sxs-lookup"><span data-stu-id="f4cd0-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="f4cd0-115">registriert</span><span class="sxs-lookup"><span data-stu-id="f4cd0-115">enrolled</span></span>|<span data-ttu-id="f4cd0-116">1</span><span class="sxs-lookup"><span data-stu-id="f4cd0-116">1</span></span>|<span data-ttu-id="f4cd0-117">Gerät ist registriert.</span><span class="sxs-lookup"><span data-stu-id="f4cd0-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="f4cd0-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="f4cd0-118">pendingReset</span></span>|<span data-ttu-id="f4cd0-119">2</span><span class="sxs-lookup"><span data-stu-id="f4cd0-119">2</span></span>|<span data-ttu-id="f4cd0-120">Registriert, aber es über Registrierung Profil registriert ist und das registrierte Profil unterscheidet sich von der zugewiesenen Profil.</span><span class="sxs-lookup"><span data-stu-id="f4cd0-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="f4cd0-121">failed</span><span class="sxs-lookup"><span data-stu-id="f4cd0-121">failed</span></span>|<span data-ttu-id="f4cd0-122">3</span><span class="sxs-lookup"><span data-stu-id="f4cd0-122">3</span></span>|<span data-ttu-id="f4cd0-123">Nicht registriert und Registrierung Fehler Datensatz vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="f4cd0-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="f4cd0-124">notContacted</span><span class="sxs-lookup"><span data-stu-id="f4cd0-124">notContacted</span></span>|<span data-ttu-id="f4cd0-125">4</span><span class="sxs-lookup"><span data-stu-id="f4cd0-125">4</span></span>|<span data-ttu-id="f4cd0-126">Gerät ist importiert, aber nicht registriert.</span><span class="sxs-lookup"><span data-stu-id="f4cd0-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="f4cd0-127">gesperrt</span><span class="sxs-lookup"><span data-stu-id="f4cd0-127">blocked</span></span>|<span data-ttu-id="f4cd0-128">5</span><span class="sxs-lookup"><span data-stu-id="f4cd0-128">5</span></span>|<span data-ttu-id="f4cd0-129">Gerät als userless registriert ist, aber wird blockiert zu Benutzer Registrierung navigieren, da die app konnte nicht installiert werden.</span><span class="sxs-lookup"><span data-stu-id="f4cd0-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|





