---
title: IVR-Szenarien in Anrufe
description: 'Im folgenden sind die interaktive Sprachantwort (IVR) Szenarien, die der aufrufende APIs in Microsoft Graph zu unterstützen:'
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 014fd2169678617043a5a540f625479e68302b34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855811"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="8c3ce-103">IVR-Szenarien in Anrufe</span><span class="sxs-lookup"><span data-stu-id="8c3ce-103">IVR scenarios in calls</span></span>

> <span data-ttu-id="8c3ce-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8c3ce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c3ce-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8c3ce-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8c3ce-106">Im folgenden sind die interaktive Sprachantwort (IVR) Szenarien, die der aufrufende APIs in Microsoft Graph zu unterstützen:</span><span class="sxs-lookup"><span data-stu-id="8c3ce-106">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="8c3ce-107">Wiedergabe einer audioansage - beispielsweise, wenn ein Anruf in einem Kundenservice-Mitarbeiterin Warteschlange platziert wird.</span><span class="sxs-lookup"><span data-stu-id="8c3ce-107">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="8c3ce-108">Datensatz - beispielsweise auf das Audio des Anrufers, notieren Sie in der Regel, nachdem sie eine Aufforderung mit Optionen hören.</span><span class="sxs-lookup"><span data-stu-id="8c3ce-108">Record - for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="8c3ce-109">Tone - beispielsweise abonnieren, wenn Sie wissen, welche DTMF möchten Klingeltöne des Aufrufers ausgewählt haben, in der Regel nach der audioansage hören.</span><span class="sxs-lookup"><span data-stu-id="8c3ce-109">Subscribe to tone - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="8c3ce-110">Brechen Sie Medienverarbeitung - beispielsweise ab, wenn Sie alle Vorgänge PlayPrompt oder Datensatz Abbrechen, die im Prozess möglicherweise möchten.</span><span class="sxs-lookup"><span data-stu-id="8c3ce-110">Cancel Media Processing - for example, when you want to cancel any PlayPrompt or Record operations that might be in process.</span></span>
