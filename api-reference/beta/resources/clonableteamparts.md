---
title: ClonableTeamParts Enum-Typ
description: 'Beschreibt, welche Teil eines Teams geklont werden soll. '
ms.openlocfilehash: 123cdb5ff7fd4a4291df5d9352b0db466908cc3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059479"
---
# <a name="clonableteamparts-enum-type"></a><span data-ttu-id="72dd9-103">ClonableTeamParts Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="72dd9-103">clonableTeamParts enum type</span></span>

> <span data-ttu-id="72dd9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="72dd9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72dd9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="72dd9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="72dd9-106">Beschreibt, welche Teil eines [Team](../resources/team.md) geklont werden soll.</span><span class="sxs-lookup"><span data-stu-id="72dd9-106">Describes which part of a [team](../resources/team.md) should be cloned.</span></span> 

## <a name="members"></a><span data-ttu-id="72dd9-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="72dd9-107">Members</span></span>

| <span data-ttu-id="72dd9-108">Element</span><span class="sxs-lookup"><span data-stu-id="72dd9-108">Member</span></span> | <span data-ttu-id="72dd9-109">Wert</span><span class="sxs-lookup"><span data-stu-id="72dd9-109">Value</span></span>| <span data-ttu-id="72dd9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72dd9-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="72dd9-111">Apps</span><span class="sxs-lookup"><span data-stu-id="72dd9-111">apps</span></span>|<span data-ttu-id="72dd9-112">1</span><span class="sxs-lookup"><span data-stu-id="72dd9-112">1</span></span>|<span data-ttu-id="72dd9-113">Kopieren Sie die Liste der installierten apps.</span><span class="sxs-lookup"><span data-stu-id="72dd9-113">Copy the list of installed apps.</span></span>|
|<span data-ttu-id="72dd9-114">Registerkarten</span><span class="sxs-lookup"><span data-stu-id="72dd9-114">tabs</span></span>|<span data-ttu-id="72dd9-115">2</span><span class="sxs-lookup"><span data-stu-id="72dd9-115">2</span></span>|<span data-ttu-id="72dd9-116">die Registerkarten in den Kanälen kopiert.</span><span class="sxs-lookup"><span data-stu-id="72dd9-116">copies the tabs within channels.</span></span>|
|<span data-ttu-id="72dd9-117">settings</span><span class="sxs-lookup"><span data-stu-id="72dd9-117">settings</span></span>|<span data-ttu-id="72dd9-118">4</span><span class="sxs-lookup"><span data-stu-id="72dd9-118">4</span></span>|<span data-ttu-id="72dd9-119">Kopiert alle Einstellungen im Team, zusammen mit den wichtigsten gruppeneinstellungen.</span><span class="sxs-lookup"><span data-stu-id="72dd9-119">Copies all settings within the team, along with key group settings.</span></span>|
|<span data-ttu-id="72dd9-120">Kanäle</span><span class="sxs-lookup"><span data-stu-id="72dd9-120">channels</span></span>|<span data-ttu-id="72dd9-121">8</span><span class="sxs-lookup"><span data-stu-id="72dd9-121">8</span></span>|<span data-ttu-id="72dd9-122">kopiert die Struktur DDE-Kanal (jedoch nicht die Nachrichten im Kanal).</span><span class="sxs-lookup"><span data-stu-id="72dd9-122">copies the channel structure (but not the messages in the channel).</span></span>|
|<span data-ttu-id="72dd9-123">Elemente</span><span class="sxs-lookup"><span data-stu-id="72dd9-123">members</span></span>|<span data-ttu-id="72dd9-124">16</span><span class="sxs-lookup"><span data-stu-id="72dd9-124">16</span></span>|<span data-ttu-id="72dd9-125">kopiert die Elemente und Besitzer des Teams.</span><span class="sxs-lookup"><span data-stu-id="72dd9-125">copies the members and owners of the team.</span></span>|
