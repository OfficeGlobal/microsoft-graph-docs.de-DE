---
title: EnrollmentState Enum-Typ
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b71f41d459e3fdb50fd853c62a855b4591a8ca8e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419107"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="1ef62-103">EnrollmentState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="1ef62-103">enrollmentState enum type</span></span>

> <span data-ttu-id="1ef62-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="1ef62-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1ef62-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1ef62-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1ef62-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1ef62-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ef62-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1ef62-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="1ef62-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="1ef62-108">Members</span></span>
|<span data-ttu-id="1ef62-109">Member</span><span class="sxs-lookup"><span data-stu-id="1ef62-109">Member</span></span>|<span data-ttu-id="1ef62-110">Wert</span><span class="sxs-lookup"><span data-stu-id="1ef62-110">Value</span></span>|<span data-ttu-id="1ef62-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1ef62-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ef62-112">unknown</span><span class="sxs-lookup"><span data-stu-id="1ef62-112">unknown</span></span>|<span data-ttu-id="1ef62-113">0</span><span class="sxs-lookup"><span data-stu-id="1ef62-113">0</span></span>|<span data-ttu-id="1ef62-114">Die Registrierung des Geräts ist unbekannt</span><span class="sxs-lookup"><span data-stu-id="1ef62-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="1ef62-115">registriert</span><span class="sxs-lookup"><span data-stu-id="1ef62-115">enrolled</span></span>|<span data-ttu-id="1ef62-116">1</span><span class="sxs-lookup"><span data-stu-id="1ef62-116">1</span></span>|<span data-ttu-id="1ef62-117">Gerät ist registriert.</span><span class="sxs-lookup"><span data-stu-id="1ef62-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="1ef62-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="1ef62-118">pendingReset</span></span>|<span data-ttu-id="1ef62-119">2</span><span class="sxs-lookup"><span data-stu-id="1ef62-119">2</span></span>|<span data-ttu-id="1ef62-120">Registriert, aber es über Registrierung Profil registriert ist und das registrierte Profil unterscheidet sich von der zugewiesenen Profil.</span><span class="sxs-lookup"><span data-stu-id="1ef62-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="1ef62-121">failed</span><span class="sxs-lookup"><span data-stu-id="1ef62-121">failed</span></span>|<span data-ttu-id="1ef62-122">3</span><span class="sxs-lookup"><span data-stu-id="1ef62-122">3</span></span>|<span data-ttu-id="1ef62-123">Nicht registriert und Registrierung Fehler Datensatz vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="1ef62-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="1ef62-124">notContacted</span><span class="sxs-lookup"><span data-stu-id="1ef62-124">notContacted</span></span>|<span data-ttu-id="1ef62-125">4</span><span class="sxs-lookup"><span data-stu-id="1ef62-125">4</span></span>|<span data-ttu-id="1ef62-126">Gerät ist importiert, aber nicht registriert.</span><span class="sxs-lookup"><span data-stu-id="1ef62-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="1ef62-127">gesperrt</span><span class="sxs-lookup"><span data-stu-id="1ef62-127">blocked</span></span>|<span data-ttu-id="1ef62-128">5</span><span class="sxs-lookup"><span data-stu-id="1ef62-128">5</span></span>|<span data-ttu-id="1ef62-129">Gerät als userless registriert ist, aber wird blockiert zu Benutzer Registrierung navigieren, da die app konnte nicht installiert werden.</span><span class="sxs-lookup"><span data-stu-id="1ef62-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|




