---
title: DiagnosticDataSubmissionMode Enum-Typ
description: Zulassen Sie das Gerät zum Senden von Diagnose- und Verwendungsanalyse Telemetriedaten wie Watson.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: a293288c3891f8ecd77d422986e419d2e3d53767
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912946"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="023e8-103">DiagnosticDataSubmissionMode Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="023e8-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="023e8-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="023e8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="023e8-105">Zulassen Sie das Gerät zum Senden von Diagnose- und Verwendungsanalyse Telemetriedaten wie Watson.</span><span class="sxs-lookup"><span data-stu-id="023e8-105">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>
## <a name="members"></a><span data-ttu-id="023e8-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="023e8-106">Members</span></span>
|<span data-ttu-id="023e8-107">Element</span><span class="sxs-lookup"><span data-stu-id="023e8-107">Member</span></span>|<span data-ttu-id="023e8-108">Wert</span><span class="sxs-lookup"><span data-stu-id="023e8-108">Value</span></span>|<span data-ttu-id="023e8-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="023e8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="023e8-110">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="023e8-110">userDefined</span></span>|<span data-ttu-id="023e8-111">0</span><span class="sxs-lookup"><span data-stu-id="023e8-111">0</span></span>|<span data-ttu-id="023e8-112">Ermöglicht es dem Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="023e8-112">Allow the user to set.</span></span>|
|<span data-ttu-id="023e8-113">n/v</span><span class="sxs-lookup"><span data-stu-id="023e8-113">none</span></span>|<span data-ttu-id="023e8-114">1</span><span class="sxs-lookup"><span data-stu-id="023e8-114">1</span></span>|<span data-ttu-id="023e8-115">Keine Telemetriedaten werden von Betriebssystemkomponenten gesendet.</span><span class="sxs-lookup"><span data-stu-id="023e8-115">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="023e8-116">Hinweis: Dieser Wert gilt nur für Enterprise und Server-Geräte.</span><span class="sxs-lookup"><span data-stu-id="023e8-116">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="023e8-117">Mit dieser Einstellung auf anderen Geräten entspricht dem Festlegen des Werts von 1.</span><span class="sxs-lookup"><span data-stu-id="023e8-117">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="023e8-118">grundlegende</span><span class="sxs-lookup"><span data-stu-id="023e8-118">basic</span></span>|<span data-ttu-id="023e8-119">2</span><span class="sxs-lookup"><span data-stu-id="023e8-119">2</span></span>|<span data-ttu-id="023e8-120">Grundlegende Telemetriedaten sendet.</span><span class="sxs-lookup"><span data-stu-id="023e8-120">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="023e8-121">Erweiterte</span><span class="sxs-lookup"><span data-stu-id="023e8-121">enhanced</span></span>|<span data-ttu-id="023e8-122">3</span><span class="sxs-lookup"><span data-stu-id="023e8-122">3</span></span>|<span data-ttu-id="023e8-123">Sendet erweiterten Telemetriedaten, einschließlich der Verwendung und Einblicke in die Daten.</span><span class="sxs-lookup"><span data-stu-id="023e8-123">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="023e8-124">vollständige</span><span class="sxs-lookup"><span data-stu-id="023e8-124">full</span></span>|<span data-ttu-id="023e8-125">4</span><span class="sxs-lookup"><span data-stu-id="023e8-125">4</span></span>|<span data-ttu-id="023e8-126">Sendet vollständige Telemetriedaten einschließlich Diagnosedaten wie Systemstatus.</span><span class="sxs-lookup"><span data-stu-id="023e8-126">Sends full telemetry data including diagnostic data, such as system state.</span></span>|



