---
title: edgeTelemetryMode-Enumerationstyp
description: Art der durchsuchten Daten, die an Microsoft 365 Analytics gesendet werden
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b48840debffcc7aedf1454d9cee11b6c0ab9edc1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172471"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="62a3d-103">edgeTelemetryMode-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="62a3d-103">edgeTelemetryMode enum type</span></span>

> <span data-ttu-id="62a3d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="62a3d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62a3d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="62a3d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62a3d-106">Art der durchsuchten Daten, die an Microsoft 365 Analytics gesendet werden</span><span class="sxs-lookup"><span data-stu-id="62a3d-106">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="62a3d-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="62a3d-107">Members</span></span>
|<span data-ttu-id="62a3d-108">Element</span><span class="sxs-lookup"><span data-stu-id="62a3d-108">Member</span></span>|<span data-ttu-id="62a3d-109">Wert</span><span class="sxs-lookup"><span data-stu-id="62a3d-109">Value</span></span>|<span data-ttu-id="62a3d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62a3d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62a3d-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="62a3d-111">notConfigured</span></span>|<span data-ttu-id="62a3d-112">0</span><span class="sxs-lookup"><span data-stu-id="62a3d-112">0</span></span>|<span data-ttu-id="62a3d-113">Standard – keine Telemetrie-Daten erfasst oder gesendet</span><span class="sxs-lookup"><span data-stu-id="62a3d-113">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="62a3d-114">Intranet</span><span class="sxs-lookup"><span data-stu-id="62a3d-114">intranet</span></span>|<span data-ttu-id="62a3d-115">1</span><span class="sxs-lookup"><span data-stu-id="62a3d-115">1</span></span>|<span data-ttu-id="62a3d-116">Nur Senden des Intranet-Verlaufs zulassen: nur Senden von Browserverlaufsdaten für Intranet-Websites</span><span class="sxs-lookup"><span data-stu-id="62a3d-116">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="62a3d-117">internet</span><span class="sxs-lookup"><span data-stu-id="62a3d-117">internet</span></span>|<span data-ttu-id="62a3d-118">2</span><span class="sxs-lookup"><span data-stu-id="62a3d-118">2</span></span>|<span data-ttu-id="62a3d-119">Nur Senden des Internet Verlaufs zulassen: nur Browserverlaufsdaten für Internetwebsites senden</span><span class="sxs-lookup"><span data-stu-id="62a3d-119">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="62a3d-120">intranetAndInternet</span><span class="sxs-lookup"><span data-stu-id="62a3d-120">intranetAndInternet</span></span>|<span data-ttu-id="62a3d-121">3</span><span class="sxs-lookup"><span data-stu-id="62a3d-121">3</span></span>|<span data-ttu-id="62a3d-122">Senden von Intranet-und Internetprotokollen: Senden von Browserverlaufsdaten für Intranet-und Internetwebsites</span><span class="sxs-lookup"><span data-stu-id="62a3d-122">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|




