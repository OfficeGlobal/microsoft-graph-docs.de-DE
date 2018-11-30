---
title: DefenderPromptForSampleSubmission Enum-Typ
description: Mögliche Werte für den Benutzer für die Übermittlung Beispiele.
ms.openlocfilehash: b70e86cb010395d5c3dfbd3266cc0cb7f6383fbd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059907"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="c7497-103">DefenderPromptForSampleSubmission Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="c7497-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="c7497-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c7497-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7497-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c7497-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7497-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c7497-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7497-107">Mögliche Werte für den Benutzer für die Übermittlung Beispiele.</span><span class="sxs-lookup"><span data-stu-id="c7497-107">Possible values for prompting user for samples submission.</span></span>
## <a name="members"></a><span data-ttu-id="c7497-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="c7497-108">Members</span></span>
|<span data-ttu-id="c7497-109">Element</span><span class="sxs-lookup"><span data-stu-id="c7497-109">Member</span></span>|<span data-ttu-id="c7497-110">Wert</span><span class="sxs-lookup"><span data-stu-id="c7497-110">Value</span></span>|<span data-ttu-id="c7497-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7497-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7497-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="c7497-112">userDefined</span></span>|<span data-ttu-id="c7497-113">0</span><span class="sxs-lookup"><span data-stu-id="c7497-113">0</span></span>|<span data-ttu-id="c7497-114">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="c7497-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="c7497-115">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="c7497-115">alwaysPrompt</span></span>|<span data-ttu-id="c7497-116">1</span><span class="sxs-lookup"><span data-stu-id="c7497-116">1</span></span>|<span data-ttu-id="c7497-117">Immer auffordern.</span><span class="sxs-lookup"><span data-stu-id="c7497-117">Always prompt.</span></span>|
|<span data-ttu-id="c7497-118">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="c7497-118">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="c7497-119">2</span><span class="sxs-lookup"><span data-stu-id="c7497-119">2</span></span>|<span data-ttu-id="c7497-120">Auffordern Sie, vor dem Senden von persönlicher Daten.</span><span class="sxs-lookup"><span data-stu-id="c7497-120">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="c7497-121">neverSendData</span><span class="sxs-lookup"><span data-stu-id="c7497-121">neverSendData</span></span>|<span data-ttu-id="c7497-122">3</span><span class="sxs-lookup"><span data-stu-id="c7497-122">3</span></span>|<span data-ttu-id="c7497-123">Nie senden Daten an.</span><span class="sxs-lookup"><span data-stu-id="c7497-123">Never send data.</span></span>|
|<span data-ttu-id="c7497-124">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="c7497-124">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="c7497-125">4</span><span class="sxs-lookup"><span data-stu-id="c7497-125">4</span></span>|<span data-ttu-id="c7497-126">Alle Daten ohne entsprechende Benachrichtigung gesendet.</span><span class="sxs-lookup"><span data-stu-id="c7497-126">Send all data without prompting.</span></span>|





