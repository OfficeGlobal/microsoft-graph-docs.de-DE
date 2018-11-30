---
title: IVR-Szenarien in Anrufe
description: 'Im folgenden sind die interaktive Sprachantwort (IVR) Szenarien, die der aufrufende APIs in Microsoft Graph zu unterstützen:'
ms.openlocfilehash: 22318b2bc755b161a55fc42fd924017545d38e3b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058225"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="c7a57-103">IVR-Szenarien in Anrufe</span><span class="sxs-lookup"><span data-stu-id="c7a57-103">IVR scenarios in calls</span></span>

> <span data-ttu-id="c7a57-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c7a57-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7a57-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c7a57-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c7a57-106">Im folgenden sind die interaktive Sprachantwort (IVR) Szenarien, die der aufrufende APIs in Microsoft Graph zu unterstützen:</span><span class="sxs-lookup"><span data-stu-id="c7a57-106">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="c7a57-107">Wiedergabe einer audioansage - beispielsweise, wenn ein Anruf in einem Kundenservice-Mitarbeiterin Warteschlange platziert wird.</span><span class="sxs-lookup"><span data-stu-id="c7a57-107">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="c7a57-108">Datensatz - beispielsweise auf das Audio des Anrufers, notieren Sie in der Regel, nachdem sie eine Aufforderung mit Optionen hören.</span><span class="sxs-lookup"><span data-stu-id="c7a57-108">Record - for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="c7a57-109">Tone - beispielsweise abonnieren, wenn Sie wissen, welche DTMF möchten Klingeltöne des Aufrufers ausgewählt haben, in der Regel nach der audioansage hören.</span><span class="sxs-lookup"><span data-stu-id="c7a57-109">Subscribe to tone - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="c7a57-110">Brechen Sie Medienverarbeitung - beispielsweise ab, wenn Sie alle Vorgänge PlayPrompt oder Datensatz Abbrechen, die im Prozess möglicherweise möchten.</span><span class="sxs-lookup"><span data-stu-id="c7a57-110">Cancel Media Processing - for example, when you want to cancel any PlayPrompt or Record operations that might be in process.</span></span>
