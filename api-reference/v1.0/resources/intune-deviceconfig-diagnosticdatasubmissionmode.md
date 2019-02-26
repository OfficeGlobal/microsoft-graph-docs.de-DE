---
title: diagnosticDataSubmissionMode-Enumerationstyp
description: Das Gerät kann Diagnose-und Verwendungs Telemetrie-Daten wie Watson senden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c0707b97e60da406210d6a091ed0dd4efaa2299
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251034"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="7c918-103">diagnosticDataSubmissionMode-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="7c918-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="7c918-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7c918-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c918-105">Das Gerät kann Diagnose-und Verwendungs Telemetrie-Daten wie Watson senden.</span><span class="sxs-lookup"><span data-stu-id="7c918-105">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="7c918-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="7c918-106">Members</span></span>
|<span data-ttu-id="7c918-107">Element</span><span class="sxs-lookup"><span data-stu-id="7c918-107">Member</span></span>|<span data-ttu-id="7c918-108">Wert</span><span class="sxs-lookup"><span data-stu-id="7c918-108">Value</span></span>|<span data-ttu-id="7c918-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c918-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c918-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="7c918-110">userDefined</span></span>|<span data-ttu-id="7c918-111">0</span><span class="sxs-lookup"><span data-stu-id="7c918-111">0</span></span>|<span data-ttu-id="7c918-112">Zulassen, dass der Benutzer festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="7c918-112">Allow the user to set.</span></span>|
|<span data-ttu-id="7c918-113">Keine</span><span class="sxs-lookup"><span data-stu-id="7c918-113">none</span></span>|<span data-ttu-id="7c918-114">1</span><span class="sxs-lookup"><span data-stu-id="7c918-114">1</span></span>|<span data-ttu-id="7c918-115">Von Betriebssystemkomponenten werden keine Telemetrie-Daten gesendet.</span><span class="sxs-lookup"><span data-stu-id="7c918-115">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="7c918-116">Hinweis: dieser Wert gilt nur für Enterprise-und Server-Geräte.</span><span class="sxs-lookup"><span data-stu-id="7c918-116">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="7c918-117">Die Verwendung dieser Einstellung auf anderen Geräten entspricht dem Festlegen des Werts 1.</span><span class="sxs-lookup"><span data-stu-id="7c918-117">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="7c918-118">Basic</span><span class="sxs-lookup"><span data-stu-id="7c918-118">basic</span></span>|<span data-ttu-id="7c918-119">2</span><span class="sxs-lookup"><span data-stu-id="7c918-119">2</span></span>|<span data-ttu-id="7c918-120">Sendet grundlegende Telemetrie-Daten.</span><span class="sxs-lookup"><span data-stu-id="7c918-120">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="7c918-121">Erweiterte</span><span class="sxs-lookup"><span data-stu-id="7c918-121">enhanced</span></span>|<span data-ttu-id="7c918-122">3</span><span class="sxs-lookup"><span data-stu-id="7c918-122">3</span></span>|<span data-ttu-id="7c918-123">Sendet erweiterte Telemetrie-Daten, einschließlich Verwendungs-und einblickdaten.</span><span class="sxs-lookup"><span data-stu-id="7c918-123">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="7c918-124">vollständige</span><span class="sxs-lookup"><span data-stu-id="7c918-124">full</span></span>|<span data-ttu-id="7c918-125">4</span><span class="sxs-lookup"><span data-stu-id="7c918-125">4</span></span>|<span data-ttu-id="7c918-126">Sendet vollständige Telemetrie-Daten einschließlich Diagnosedaten wie Systemstatus.</span><span class="sxs-lookup"><span data-stu-id="7c918-126">Sends full telemetry data including diagnostic data, such as system state.</span></span>|



