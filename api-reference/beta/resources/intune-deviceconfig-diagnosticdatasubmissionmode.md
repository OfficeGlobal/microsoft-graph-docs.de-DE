---
title: DiagnosticDataSubmissionMode Enum-Typ
description: Zulassen Sie das Gerät zum Senden von Diagnose- und Verwendungsanalyse Telemetriedaten wie Watson.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: d1ba4d2cd9be740b23502ec4c0154caa2be07f3c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948529"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="56b3a-103">DiagnosticDataSubmissionMode Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="56b3a-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="56b3a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="56b3a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56b3a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="56b3a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56b3a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="56b3a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56b3a-107">Zulassen Sie das Gerät zum Senden von Diagnose- und Verwendungsanalyse Telemetriedaten wie Watson.</span><span class="sxs-lookup"><span data-stu-id="56b3a-107">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>
## <a name="members"></a><span data-ttu-id="56b3a-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="56b3a-108">Members</span></span>
|<span data-ttu-id="56b3a-109">Element</span><span class="sxs-lookup"><span data-stu-id="56b3a-109">Member</span></span>|<span data-ttu-id="56b3a-110">Wert</span><span class="sxs-lookup"><span data-stu-id="56b3a-110">Value</span></span>|<span data-ttu-id="56b3a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56b3a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56b3a-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="56b3a-112">userDefined</span></span>|<span data-ttu-id="56b3a-113">0</span><span class="sxs-lookup"><span data-stu-id="56b3a-113">0</span></span>|<span data-ttu-id="56b3a-114">Ermöglicht es dem Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="56b3a-114">Allow the user to set.</span></span>|
|<span data-ttu-id="56b3a-115">n/v</span><span class="sxs-lookup"><span data-stu-id="56b3a-115">none</span></span>|<span data-ttu-id="56b3a-116">1</span><span class="sxs-lookup"><span data-stu-id="56b3a-116">1</span></span>|<span data-ttu-id="56b3a-117">Keine Telemetriedaten werden von Betriebssystemkomponenten gesendet.</span><span class="sxs-lookup"><span data-stu-id="56b3a-117">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="56b3a-118">Hinweis: Dieser Wert gilt nur für Enterprise und Server-Geräte.</span><span class="sxs-lookup"><span data-stu-id="56b3a-118">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="56b3a-119">Mit dieser Einstellung auf anderen Geräten entspricht dem Festlegen des Werts von 1.</span><span class="sxs-lookup"><span data-stu-id="56b3a-119">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="56b3a-120">grundlegende</span><span class="sxs-lookup"><span data-stu-id="56b3a-120">basic</span></span>|<span data-ttu-id="56b3a-121">2</span><span class="sxs-lookup"><span data-stu-id="56b3a-121">2</span></span>|<span data-ttu-id="56b3a-122">Grundlegende Telemetriedaten sendet.</span><span class="sxs-lookup"><span data-stu-id="56b3a-122">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="56b3a-123">Erweiterte</span><span class="sxs-lookup"><span data-stu-id="56b3a-123">enhanced</span></span>|<span data-ttu-id="56b3a-124">3</span><span class="sxs-lookup"><span data-stu-id="56b3a-124">3</span></span>|<span data-ttu-id="56b3a-125">Sendet erweiterten Telemetriedaten, einschließlich der Verwendung und Einblicke in die Daten.</span><span class="sxs-lookup"><span data-stu-id="56b3a-125">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="56b3a-126">vollständige</span><span class="sxs-lookup"><span data-stu-id="56b3a-126">full</span></span>|<span data-ttu-id="56b3a-127">4</span><span class="sxs-lookup"><span data-stu-id="56b3a-127">4</span></span>|<span data-ttu-id="56b3a-128">Sendet vollständige Telemetriedaten einschließlich Diagnosedaten wie Systemstatus.</span><span class="sxs-lookup"><span data-stu-id="56b3a-128">Sends full telemetry data including diagnostic data, such as system state.</span></span>|





