---
title: DefenderMonitorFileActivity Enum-Typ
description: Mögliche Werte für die Überwachung von Dateiaktivität.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1d7b6c921ec40b53339646b2b3b0a91e2d4e8a84
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837905"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="e3f76-103">DefenderMonitorFileActivity Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="e3f76-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="e3f76-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e3f76-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3f76-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3f76-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3f76-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e3f76-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3f76-107">Mögliche Werte für die Überwachung von Dateiaktivität.</span><span class="sxs-lookup"><span data-stu-id="e3f76-107">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="e3f76-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="e3f76-108">Members</span></span>
|<span data-ttu-id="e3f76-109">Element</span><span class="sxs-lookup"><span data-stu-id="e3f76-109">Member</span></span>|<span data-ttu-id="e3f76-110">Wert</span><span class="sxs-lookup"><span data-stu-id="e3f76-110">Value</span></span>|<span data-ttu-id="e3f76-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3f76-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3f76-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="e3f76-112">userDefined</span></span>|<span data-ttu-id="e3f76-113">0</span><span class="sxs-lookup"><span data-stu-id="e3f76-113">0</span></span>|<span data-ttu-id="e3f76-114">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="e3f76-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="e3f76-115">disable</span><span class="sxs-lookup"><span data-stu-id="e3f76-115">disable</span></span>|<span data-ttu-id="e3f76-116">1</span><span class="sxs-lookup"><span data-stu-id="e3f76-116">1</span></span>|<span data-ttu-id="e3f76-117">Überwachen der Dateiaktivität zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="e3f76-117">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="e3f76-118">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="e3f76-118">monitorAllFiles</span></span>|<span data-ttu-id="e3f76-119">2</span><span class="sxs-lookup"><span data-stu-id="e3f76-119">2</span></span>|<span data-ttu-id="e3f76-120">Überwachen Sie alle Dateien.</span><span class="sxs-lookup"><span data-stu-id="e3f76-120">Monitor all files.</span></span>|
|<span data-ttu-id="e3f76-121">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="e3f76-121">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="e3f76-122">3</span><span class="sxs-lookup"><span data-stu-id="e3f76-122">3</span></span>| <span data-ttu-id="e3f76-123">Nur eingehende Dateien zu überwachen.</span><span class="sxs-lookup"><span data-stu-id="e3f76-123">Monitor incoming files only.</span></span>|
|<span data-ttu-id="e3f76-124">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="e3f76-124">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="e3f76-125">4</span><span class="sxs-lookup"><span data-stu-id="e3f76-125">4</span></span>|<span data-ttu-id="e3f76-126">Nur ausgehende Dateien zu überwachen.</span><span class="sxs-lookup"><span data-stu-id="e3f76-126">Monitor outgoing files only.</span></span>|





