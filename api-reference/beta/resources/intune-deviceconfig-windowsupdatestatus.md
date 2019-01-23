---
title: WindowsUpdateStatus Enum-Typ
description: Windows-update für Business Konfiguration Gerätestatus
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74493359eeccdbc6df1c351ecec771b5990649b6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431564"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="f208a-103">WindowsUpdateStatus Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="f208a-103">windowsUpdateStatus enum type</span></span>

> <span data-ttu-id="f208a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f208a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f208a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f208a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f208a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f208a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f208a-107">Windows-update für Business Konfiguration Gerätestatus</span><span class="sxs-lookup"><span data-stu-id="f208a-107">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="f208a-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="f208a-108">Members</span></span>
|<span data-ttu-id="f208a-109">Member</span><span class="sxs-lookup"><span data-stu-id="f208a-109">Member</span></span>|<span data-ttu-id="f208a-110">Wert</span><span class="sxs-lookup"><span data-stu-id="f208a-110">Value</span></span>|<span data-ttu-id="f208a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f208a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f208a-112">Aktuellste</span><span class="sxs-lookup"><span data-stu-id="f208a-112">upToDate</span></span>|<span data-ttu-id="f208a-113">0</span><span class="sxs-lookup"><span data-stu-id="f208a-113">0</span></span>|<span data-ttu-id="f208a-114">Es gibt keine ausstehende Updates, keine ausstehende Updates einen Neustart und keine fehlgeschlagenen Updates.</span><span class="sxs-lookup"><span data-stu-id="f208a-114">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="f208a-115">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="f208a-115">pendingInstallation</span></span>|<span data-ttu-id="f208a-116">1</span><span class="sxs-lookup"><span data-stu-id="f208a-116">1</span></span>|<span data-ttu-id="f208a-117">Es sind Updates, die die ausstehende Installation der Updates enthält, die nicht genehmigt werden.</span><span class="sxs-lookup"><span data-stu-id="f208a-117">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="f208a-118">Es sind keine ausstehenden Neustarts Updates, keine fehlgeschlagenen Updates.</span><span class="sxs-lookup"><span data-stu-id="f208a-118">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="f208a-119">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="f208a-119">pendingReboot</span></span>|<span data-ttu-id="f208a-120">2</span><span class="sxs-lookup"><span data-stu-id="f208a-120">2</span></span>|<span data-ttu-id="f208a-121">Es sind Updates, die Neustart erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="f208a-121">There are updates that requires reboot.</span></span> <span data-ttu-id="f208a-122">Es sind nicht fehlgeschlagenen Updates.</span><span class="sxs-lookup"><span data-stu-id="f208a-122">There are not failed updates.</span></span>|
|<span data-ttu-id="f208a-123">failed</span><span class="sxs-lookup"><span data-stu-id="f208a-123">failed</span></span>|<span data-ttu-id="f208a-124">3</span><span class="sxs-lookup"><span data-stu-id="f208a-124">3</span></span>|<span data-ttu-id="f208a-125">Es sind Updates konnte nicht auf dem Gerät installiert werden.</span><span class="sxs-lookup"><span data-stu-id="f208a-125">There are updates failed to install on the device.</span></span>|




