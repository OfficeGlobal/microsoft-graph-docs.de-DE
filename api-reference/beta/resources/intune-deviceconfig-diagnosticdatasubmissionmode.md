---
title: diagnosticDataSubmissionMode-Enumerationstyp
description: Das Gerät kann Diagnose-und Verwendungs Telemetrie-Daten wie Watson senden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e749d2fc7a1eb191c62fbc9db389887cdd901c27
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175220"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="b5b6b-103">diagnosticDataSubmissionMode-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="b5b6b-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="b5b6b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b5b6b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5b6b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b5b6b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5b6b-106">Das Gerät kann Diagnose-und Verwendungs Telemetrie-Daten wie Watson senden.</span><span class="sxs-lookup"><span data-stu-id="b5b6b-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="b5b6b-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="b5b6b-107">Members</span></span>
|<span data-ttu-id="b5b6b-108">Element</span><span class="sxs-lookup"><span data-stu-id="b5b6b-108">Member</span></span>|<span data-ttu-id="b5b6b-109">Wert</span><span class="sxs-lookup"><span data-stu-id="b5b6b-109">Value</span></span>|<span data-ttu-id="b5b6b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5b6b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5b6b-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="b5b6b-111">userDefined</span></span>|<span data-ttu-id="b5b6b-112">0</span><span class="sxs-lookup"><span data-stu-id="b5b6b-112">0</span></span>|<span data-ttu-id="b5b6b-113">Zulassen, dass der Benutzer festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="b5b6b-113">Allow the user to set.</span></span>|
|<span data-ttu-id="b5b6b-114">Keine</span><span class="sxs-lookup"><span data-stu-id="b5b6b-114">none</span></span>|<span data-ttu-id="b5b6b-115">1</span><span class="sxs-lookup"><span data-stu-id="b5b6b-115">1</span></span>|<span data-ttu-id="b5b6b-116">Von Betriebssystemkomponenten werden keine Telemetrie-Daten gesendet.</span><span class="sxs-lookup"><span data-stu-id="b5b6b-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="b5b6b-117">Hinweis: dieser Wert gilt nur für Enterprise-und Server-Geräte.</span><span class="sxs-lookup"><span data-stu-id="b5b6b-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="b5b6b-118">Die Verwendung dieser Einstellung auf anderen Geräten entspricht dem Festlegen des Werts 1.</span><span class="sxs-lookup"><span data-stu-id="b5b6b-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="b5b6b-119">Basic</span><span class="sxs-lookup"><span data-stu-id="b5b6b-119">basic</span></span>|<span data-ttu-id="b5b6b-120">2</span><span class="sxs-lookup"><span data-stu-id="b5b6b-120">2</span></span>|<span data-ttu-id="b5b6b-121">Sendet grundlegende Telemetrie-Daten.</span><span class="sxs-lookup"><span data-stu-id="b5b6b-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="b5b6b-122">Erweiterte</span><span class="sxs-lookup"><span data-stu-id="b5b6b-122">enhanced</span></span>|<span data-ttu-id="b5b6b-123">3</span><span class="sxs-lookup"><span data-stu-id="b5b6b-123">3</span></span>|<span data-ttu-id="b5b6b-124">Sendet erweiterte Telemetrie-Daten, einschließlich Verwendungs-und einblickdaten.</span><span class="sxs-lookup"><span data-stu-id="b5b6b-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="b5b6b-125">vollständige</span><span class="sxs-lookup"><span data-stu-id="b5b6b-125">full</span></span>|<span data-ttu-id="b5b6b-126">4</span><span class="sxs-lookup"><span data-stu-id="b5b6b-126">4</span></span>|<span data-ttu-id="b5b6b-127">Sendet vollständige Telemetrie-Daten einschließlich Diagnosedaten wie Systemstatus.</span><span class="sxs-lookup"><span data-stu-id="b5b6b-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|




