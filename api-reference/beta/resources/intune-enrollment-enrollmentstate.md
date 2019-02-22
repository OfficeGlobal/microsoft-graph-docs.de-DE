---
title: enrollmentState-Enumerationstyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dcb039563d9c45a33c4e42344fc8557dfe29b333
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159248"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="91a96-103">enrollmentState-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="91a96-103">enrollmentState enum type</span></span>

> <span data-ttu-id="91a96-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="91a96-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91a96-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="91a96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91a96-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="91a96-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="91a96-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="91a96-107">Members</span></span>
|<span data-ttu-id="91a96-108">Element</span><span class="sxs-lookup"><span data-stu-id="91a96-108">Member</span></span>|<span data-ttu-id="91a96-109">Wert</span><span class="sxs-lookup"><span data-stu-id="91a96-109">Value</span></span>|<span data-ttu-id="91a96-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91a96-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91a96-111">unknown</span><span class="sxs-lookup"><span data-stu-id="91a96-111">unknown</span></span>|<span data-ttu-id="91a96-112">0</span><span class="sxs-lookup"><span data-stu-id="91a96-112">0</span></span>|<span data-ttu-id="91a96-113">Geräte Registrierungsstatus ist unbekannt</span><span class="sxs-lookup"><span data-stu-id="91a96-113">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="91a96-114">registriert</span><span class="sxs-lookup"><span data-stu-id="91a96-114">enrolled</span></span>|<span data-ttu-id="91a96-115">1</span><span class="sxs-lookup"><span data-stu-id="91a96-115">1</span></span>|<span data-ttu-id="91a96-116">Das Gerät ist registriert.</span><span class="sxs-lookup"><span data-stu-id="91a96-116">Device is Enrolled.</span></span>|
|<span data-ttu-id="91a96-117">pendingReset</span><span class="sxs-lookup"><span data-stu-id="91a96-117">pendingReset</span></span>|<span data-ttu-id="91a96-118">2</span><span class="sxs-lookup"><span data-stu-id="91a96-118">2</span></span>|<span data-ttu-id="91a96-119">Registriert, aber es wird über das Registrierungsprofil registriert, und das registrierte Profil unterscheidet sich von dem zugewiesenen Profil.</span><span class="sxs-lookup"><span data-stu-id="91a96-119">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="91a96-120">failed</span><span class="sxs-lookup"><span data-stu-id="91a96-120">failed</span></span>|<span data-ttu-id="91a96-121">3</span><span class="sxs-lookup"><span data-stu-id="91a96-121">3</span></span>|<span data-ttu-id="91a96-122">Nicht registriert, und es gibt einen Registrierungsdatensatz.</span><span class="sxs-lookup"><span data-stu-id="91a96-122">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="91a96-123">notContacted</span><span class="sxs-lookup"><span data-stu-id="91a96-123">notContacted</span></span>|<span data-ttu-id="91a96-124">4</span><span class="sxs-lookup"><span data-stu-id="91a96-124">4</span></span>|<span data-ttu-id="91a96-125">Das Gerät wurde importiert, aber nicht registriert.</span><span class="sxs-lookup"><span data-stu-id="91a96-125">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="91a96-126">gesperrt</span><span class="sxs-lookup"><span data-stu-id="91a96-126">blocked</span></span>|<span data-ttu-id="91a96-127">5</span><span class="sxs-lookup"><span data-stu-id="91a96-127">5</span></span>|<span data-ttu-id="91a96-128">Das Gerät ist als Benutzerlos registriert, es wird jedoch verhindert, dass es zur Benutzerregistrierung wechselt, da die APP nicht installiert werden konnte.</span><span class="sxs-lookup"><span data-stu-id="91a96-128">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|




