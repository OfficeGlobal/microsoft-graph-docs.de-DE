---
title: DefenderMonitorFileActivity Enum-Typ
description: Mögliche Werte für die Überwachung von Dateiaktivität.
author: tfitzmac
ms.openlocfilehash: 32b3972f6c4c09117f3b8001038c0316235ea222
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338108"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="af46f-103">DefenderMonitorFileActivity Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="af46f-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="af46f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="af46f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af46f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="af46f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af46f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="af46f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af46f-107">Mögliche Werte für die Überwachung von Dateiaktivität.</span><span class="sxs-lookup"><span data-stu-id="af46f-107">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="af46f-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="af46f-108">Members</span></span>
|<span data-ttu-id="af46f-109">Member</span><span class="sxs-lookup"><span data-stu-id="af46f-109">Member</span></span>|<span data-ttu-id="af46f-110">Wert</span><span class="sxs-lookup"><span data-stu-id="af46f-110">Value</span></span>|<span data-ttu-id="af46f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="af46f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af46f-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="af46f-112">userDefined</span></span>|<span data-ttu-id="af46f-113">0</span><span class="sxs-lookup"><span data-stu-id="af46f-113">0</span></span>|<span data-ttu-id="af46f-114">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="af46f-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="af46f-115">Deaktivieren</span><span class="sxs-lookup"><span data-stu-id="af46f-115">disable</span></span>|<span data-ttu-id="af46f-116">1</span><span class="sxs-lookup"><span data-stu-id="af46f-116">1</span></span>|<span data-ttu-id="af46f-117">Überwachen der Dateiaktivität zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="af46f-117">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="af46f-118">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="af46f-118">monitorAllFiles</span></span>|<span data-ttu-id="af46f-119">2</span><span class="sxs-lookup"><span data-stu-id="af46f-119">2</span></span>|<span data-ttu-id="af46f-120">Überwachen Sie alle Dateien.</span><span class="sxs-lookup"><span data-stu-id="af46f-120">Monitor all files.</span></span>|
|<span data-ttu-id="af46f-121">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="af46f-121">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="af46f-122">3</span><span class="sxs-lookup"><span data-stu-id="af46f-122">3</span></span>| <span data-ttu-id="af46f-123">Nur eingehende Dateien zu überwachen.</span><span class="sxs-lookup"><span data-stu-id="af46f-123">Monitor incoming files only.</span></span>|
|<span data-ttu-id="af46f-124">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="af46f-124">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="af46f-125">4</span><span class="sxs-lookup"><span data-stu-id="af46f-125">4</span></span>|<span data-ttu-id="af46f-126">Nur ausgehende Dateien zu überwachen.</span><span class="sxs-lookup"><span data-stu-id="af46f-126">Monitor outgoing files only.</span></span>|





