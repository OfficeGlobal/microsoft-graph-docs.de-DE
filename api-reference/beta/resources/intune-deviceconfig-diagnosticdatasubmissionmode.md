---
title: DiagnosticDataSubmissionMode Enum-Typ
description: Zulassen Sie das Gerät zum Senden von Diagnose- und Verwendungsanalyse Telemetriedaten wie Watson.
localization_priority: Normal
ms.openlocfilehash: 3be69b4be25ece2ced611c028a855347e4dba66e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871533"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="4cb53-103">DiagnosticDataSubmissionMode Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="4cb53-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="4cb53-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4cb53-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4cb53-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4cb53-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4cb53-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4cb53-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4cb53-107">Zulassen Sie das Gerät zum Senden von Diagnose- und Verwendungsanalyse Telemetriedaten wie Watson.</span><span class="sxs-lookup"><span data-stu-id="4cb53-107">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>
## <a name="members"></a><span data-ttu-id="4cb53-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="4cb53-108">Members</span></span>
|<span data-ttu-id="4cb53-109">Element</span><span class="sxs-lookup"><span data-stu-id="4cb53-109">Member</span></span>|<span data-ttu-id="4cb53-110">Wert</span><span class="sxs-lookup"><span data-stu-id="4cb53-110">Value</span></span>|<span data-ttu-id="4cb53-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4cb53-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cb53-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="4cb53-112">userDefined</span></span>|<span data-ttu-id="4cb53-113">0</span><span class="sxs-lookup"><span data-stu-id="4cb53-113">0</span></span>|<span data-ttu-id="4cb53-114">Ermöglicht es dem Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="4cb53-114">Allow the user to set.</span></span>|
|<span data-ttu-id="4cb53-115">n/v</span><span class="sxs-lookup"><span data-stu-id="4cb53-115">none</span></span>|<span data-ttu-id="4cb53-116">1</span><span class="sxs-lookup"><span data-stu-id="4cb53-116">1</span></span>|<span data-ttu-id="4cb53-117">Keine Telemetriedaten werden von Betriebssystemkomponenten gesendet.</span><span class="sxs-lookup"><span data-stu-id="4cb53-117">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="4cb53-118">Hinweis: Dieser Wert gilt nur für Enterprise und Server-Geräte.</span><span class="sxs-lookup"><span data-stu-id="4cb53-118">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="4cb53-119">Mit dieser Einstellung auf anderen Geräten entspricht dem Festlegen des Werts von 1.</span><span class="sxs-lookup"><span data-stu-id="4cb53-119">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="4cb53-120">grundlegende</span><span class="sxs-lookup"><span data-stu-id="4cb53-120">basic</span></span>|<span data-ttu-id="4cb53-121">2</span><span class="sxs-lookup"><span data-stu-id="4cb53-121">2</span></span>|<span data-ttu-id="4cb53-122">Grundlegende Telemetriedaten sendet.</span><span class="sxs-lookup"><span data-stu-id="4cb53-122">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="4cb53-123">Erweiterte</span><span class="sxs-lookup"><span data-stu-id="4cb53-123">enhanced</span></span>|<span data-ttu-id="4cb53-124">3</span><span class="sxs-lookup"><span data-stu-id="4cb53-124">3</span></span>|<span data-ttu-id="4cb53-125">Sendet erweiterten Telemetriedaten, einschließlich der Verwendung und Einblicke in die Daten.</span><span class="sxs-lookup"><span data-stu-id="4cb53-125">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="4cb53-126">vollständige</span><span class="sxs-lookup"><span data-stu-id="4cb53-126">full</span></span>|<span data-ttu-id="4cb53-127">4</span><span class="sxs-lookup"><span data-stu-id="4cb53-127">4</span></span>|<span data-ttu-id="4cb53-128">Sendet vollständige Telemetriedaten einschließlich Diagnosedaten wie Systemstatus.</span><span class="sxs-lookup"><span data-stu-id="4cb53-128">Sends full telemetry data including diagnostic data, such as system state.</span></span>|





