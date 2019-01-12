---
title: VppTokenSyncStatus Enum-Typ
description: Mögliche Sync Status mit einem Apple Volume Purchase Program Token verknüpft ist.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4101f1338513787b27ce530579ffd42c7756366a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931286"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="29640-103">VppTokenSyncStatus Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="29640-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="29640-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="29640-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29640-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="29640-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29640-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="29640-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29640-107">Mögliche Sync Status mit einem Apple Volume Purchase Program Token verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="29640-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="29640-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="29640-108">Members</span></span>
|<span data-ttu-id="29640-109">Element</span><span class="sxs-lookup"><span data-stu-id="29640-109">Member</span></span>|<span data-ttu-id="29640-110">Wert</span><span class="sxs-lookup"><span data-stu-id="29640-110">Value</span></span>|<span data-ttu-id="29640-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="29640-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29640-112">n/v</span><span class="sxs-lookup"><span data-stu-id="29640-112">none</span></span>|<span data-ttu-id="29640-113">0</span><span class="sxs-lookup"><span data-stu-id="29640-113">0</span></span>|<span data-ttu-id="29640-114">Standardstatus.</span><span class="sxs-lookup"><span data-stu-id="29640-114">Default status.</span></span>|
|<span data-ttu-id="29640-115">in Bearbeitung</span><span class="sxs-lookup"><span data-stu-id="29640-115">inProgress</span></span>|<span data-ttu-id="29640-116">1</span><span class="sxs-lookup"><span data-stu-id="29640-116">1</span></span>|<span data-ttu-id="29640-117">Letzte Synchronisierung ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="29640-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="29640-118">abgeschlossen</span><span class="sxs-lookup"><span data-stu-id="29640-118">completed</span></span>|<span data-ttu-id="29640-119">2</span><span class="sxs-lookup"><span data-stu-id="29640-119">2</span></span>|<span data-ttu-id="29640-120">Letzte Synchronisierung erfolgreich abgeschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="29640-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="29640-121">failed</span><span class="sxs-lookup"><span data-stu-id="29640-121">failed</span></span>|<span data-ttu-id="29640-122">3</span><span class="sxs-lookup"><span data-stu-id="29640-122">3</span></span>|<span data-ttu-id="29640-123">Fehler bei der letzten Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="29640-123">Last Sync failed.</span></span>|





