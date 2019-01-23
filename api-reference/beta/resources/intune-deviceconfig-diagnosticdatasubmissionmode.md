---
title: DiagnosticDataSubmissionMode Enum-Typ
description: Zulassen Sie das Gerät zum Senden von Diagnose- und Verwendungsanalyse Telemetriedaten wie Watson.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b587d6872bcd3610c3b878ae7a672c3e776ea01
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422257"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="7c4f5-103">DiagnosticDataSubmissionMode Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="7c4f5-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="7c4f5-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="7c4f5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7c4f5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7c4f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7c4f5-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7c4f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c4f5-107">Zulassen Sie das Gerät zum Senden von Diagnose- und Verwendungsanalyse Telemetriedaten wie Watson.</span><span class="sxs-lookup"><span data-stu-id="7c4f5-107">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="7c4f5-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="7c4f5-108">Members</span></span>
|<span data-ttu-id="7c4f5-109">Member</span><span class="sxs-lookup"><span data-stu-id="7c4f5-109">Member</span></span>|<span data-ttu-id="7c4f5-110">Wert</span><span class="sxs-lookup"><span data-stu-id="7c4f5-110">Value</span></span>|<span data-ttu-id="7c4f5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c4f5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c4f5-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="7c4f5-112">userDefined</span></span>|<span data-ttu-id="7c4f5-113">0</span><span class="sxs-lookup"><span data-stu-id="7c4f5-113">0</span></span>|<span data-ttu-id="7c4f5-114">Ermöglicht es dem Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="7c4f5-114">Allow the user to set.</span></span>|
|<span data-ttu-id="7c4f5-115">Keine</span><span class="sxs-lookup"><span data-stu-id="7c4f5-115">none</span></span>|<span data-ttu-id="7c4f5-116">1</span><span class="sxs-lookup"><span data-stu-id="7c4f5-116">1</span></span>|<span data-ttu-id="7c4f5-117">Keine Telemetriedaten werden von Betriebssystemkomponenten gesendet.</span><span class="sxs-lookup"><span data-stu-id="7c4f5-117">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="7c4f5-118">Hinweis: Dieser Wert gilt nur für Enterprise und Server-Geräte.</span><span class="sxs-lookup"><span data-stu-id="7c4f5-118">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="7c4f5-119">Mit dieser Einstellung auf anderen Geräten entspricht dem Festlegen des Werts von 1.</span><span class="sxs-lookup"><span data-stu-id="7c4f5-119">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="7c4f5-120">grundlegende</span><span class="sxs-lookup"><span data-stu-id="7c4f5-120">basic</span></span>|<span data-ttu-id="7c4f5-121">2</span><span class="sxs-lookup"><span data-stu-id="7c4f5-121">2</span></span>|<span data-ttu-id="7c4f5-122">Grundlegende Telemetriedaten sendet.</span><span class="sxs-lookup"><span data-stu-id="7c4f5-122">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="7c4f5-123">Erweiterte</span><span class="sxs-lookup"><span data-stu-id="7c4f5-123">enhanced</span></span>|<span data-ttu-id="7c4f5-124">3</span><span class="sxs-lookup"><span data-stu-id="7c4f5-124">3</span></span>|<span data-ttu-id="7c4f5-125">Sendet erweiterten Telemetriedaten, einschließlich der Verwendung und Einblicke in die Daten.</span><span class="sxs-lookup"><span data-stu-id="7c4f5-125">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="7c4f5-126">vollständige</span><span class="sxs-lookup"><span data-stu-id="7c4f5-126">full</span></span>|<span data-ttu-id="7c4f5-127">4</span><span class="sxs-lookup"><span data-stu-id="7c4f5-127">4</span></span>|<span data-ttu-id="7c4f5-128">Sendet vollständige Telemetriedaten einschließlich Diagnosedaten wie Systemstatus.</span><span class="sxs-lookup"><span data-stu-id="7c4f5-128">Sends full telemetry data including diagnostic data, such as system state.</span></span>|




