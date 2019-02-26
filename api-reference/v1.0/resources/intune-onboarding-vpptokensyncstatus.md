---
title: vppTokenSyncStatus-Enumerationstyp
description: Möglicher Synchronisierungsstatus, der einem Apple Volume Purchase Program-Token zugeordnet ist.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6938fd41b6cd7c089b08edb629bc1197ec47c2d7
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254051"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="cfaf3-103">vppTokenSyncStatus-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="cfaf3-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="cfaf3-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="cfaf3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfaf3-105">Möglicher Synchronisierungsstatus, der einem Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="cfaf3-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="cfaf3-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="cfaf3-106">Members</span></span>
|<span data-ttu-id="cfaf3-107">Element</span><span class="sxs-lookup"><span data-stu-id="cfaf3-107">Member</span></span>|<span data-ttu-id="cfaf3-108">Wert</span><span class="sxs-lookup"><span data-stu-id="cfaf3-108">Value</span></span>|<span data-ttu-id="cfaf3-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cfaf3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfaf3-110">Keine</span><span class="sxs-lookup"><span data-stu-id="cfaf3-110">none</span></span>|<span data-ttu-id="cfaf3-111">0</span><span class="sxs-lookup"><span data-stu-id="cfaf3-111">0</span></span>|<span data-ttu-id="cfaf3-112">Standardstatus.</span><span class="sxs-lookup"><span data-stu-id="cfaf3-112">Default status.</span></span>|
|<span data-ttu-id="cfaf3-113">inProgress</span><span class="sxs-lookup"><span data-stu-id="cfaf3-113">inProgress</span></span>|<span data-ttu-id="cfaf3-114">1</span><span class="sxs-lookup"><span data-stu-id="cfaf3-114">1</span></span>|<span data-ttu-id="cfaf3-115">Letzte Synchronisierung wird ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="cfaf3-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="cfaf3-116">abgeschlossen</span><span class="sxs-lookup"><span data-stu-id="cfaf3-116">completed</span></span>|<span data-ttu-id="cfaf3-117">2</span><span class="sxs-lookup"><span data-stu-id="cfaf3-117">2</span></span>|<span data-ttu-id="cfaf3-118">Letzte Synchronisierung erfolgreich abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="cfaf3-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="cfaf3-119">failed</span><span class="sxs-lookup"><span data-stu-id="cfaf3-119">failed</span></span>|<span data-ttu-id="cfaf3-120">3</span><span class="sxs-lookup"><span data-stu-id="cfaf3-120">3</span></span>|<span data-ttu-id="cfaf3-121">Fehler bei der letzten Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="cfaf3-121">Last Sync failed.</span></span>|



