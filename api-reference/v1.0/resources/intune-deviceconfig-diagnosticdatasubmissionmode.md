---
title: DiagnosticDataSubmissionMode Enum-Typ
description: Zulassen Sie das Gerät zum Senden von Diagnose- und Verwendungsanalyse Telemetriedaten wie Watson.
localization_priority: Normal
ms.openlocfilehash: 1654e9c5c94fd79bbda0d77ef84101fb9fb92d5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812782"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="3ba1a-103">DiagnosticDataSubmissionMode Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="3ba1a-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="3ba1a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3ba1a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3ba1a-105">Zulassen Sie das Gerät zum Senden von Diagnose- und Verwendungsanalyse Telemetriedaten wie Watson.</span><span class="sxs-lookup"><span data-stu-id="3ba1a-105">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>
## <a name="members"></a><span data-ttu-id="3ba1a-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="3ba1a-106">Members</span></span>
|<span data-ttu-id="3ba1a-107">Element</span><span class="sxs-lookup"><span data-stu-id="3ba1a-107">Member</span></span>|<span data-ttu-id="3ba1a-108">Wert</span><span class="sxs-lookup"><span data-stu-id="3ba1a-108">Value</span></span>|<span data-ttu-id="3ba1a-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ba1a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ba1a-110">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="3ba1a-110">userDefined</span></span>|<span data-ttu-id="3ba1a-111">0</span><span class="sxs-lookup"><span data-stu-id="3ba1a-111">0</span></span>|<span data-ttu-id="3ba1a-112">Ermöglicht es dem Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="3ba1a-112">Allow the user to set.</span></span>|
|<span data-ttu-id="3ba1a-113">n/v</span><span class="sxs-lookup"><span data-stu-id="3ba1a-113">none</span></span>|<span data-ttu-id="3ba1a-114">1</span><span class="sxs-lookup"><span data-stu-id="3ba1a-114">1</span></span>|<span data-ttu-id="3ba1a-115">Keine Telemetriedaten werden von Betriebssystemkomponenten gesendet.</span><span class="sxs-lookup"><span data-stu-id="3ba1a-115">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="3ba1a-116">Hinweis: Dieser Wert gilt nur für Enterprise und Server-Geräte.</span><span class="sxs-lookup"><span data-stu-id="3ba1a-116">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="3ba1a-117">Mit dieser Einstellung auf anderen Geräten entspricht dem Festlegen des Werts von 1.</span><span class="sxs-lookup"><span data-stu-id="3ba1a-117">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="3ba1a-118">grundlegende</span><span class="sxs-lookup"><span data-stu-id="3ba1a-118">basic</span></span>|<span data-ttu-id="3ba1a-119">2</span><span class="sxs-lookup"><span data-stu-id="3ba1a-119">2</span></span>|<span data-ttu-id="3ba1a-120">Grundlegende Telemetriedaten sendet.</span><span class="sxs-lookup"><span data-stu-id="3ba1a-120">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="3ba1a-121">Erweiterte</span><span class="sxs-lookup"><span data-stu-id="3ba1a-121">enhanced</span></span>|<span data-ttu-id="3ba1a-122">3</span><span class="sxs-lookup"><span data-stu-id="3ba1a-122">3</span></span>|<span data-ttu-id="3ba1a-123">Sendet erweiterten Telemetriedaten, einschließlich der Verwendung und Einblicke in die Daten.</span><span class="sxs-lookup"><span data-stu-id="3ba1a-123">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="3ba1a-124">vollständige</span><span class="sxs-lookup"><span data-stu-id="3ba1a-124">full</span></span>|<span data-ttu-id="3ba1a-125">4</span><span class="sxs-lookup"><span data-stu-id="3ba1a-125">4</span></span>|<span data-ttu-id="3ba1a-126">Sendet vollständige Telemetriedaten einschließlich Diagnosedaten wie Systemstatus.</span><span class="sxs-lookup"><span data-stu-id="3ba1a-126">Sends full telemetry data including diagnostic data, such as system state.</span></span>|



