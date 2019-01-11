---
title: ClonableTeamParts Enum-Typ
description: 'Beschreibt, welche Teil eines Teams geklont werden soll. '
localization_priority: Normal
ms.openlocfilehash: 7eb71de266ea4f0ed9f94900dd03a47da1a24cc1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860557"
---
# <a name="clonableteamparts-enum-type"></a><span data-ttu-id="c5f74-103">ClonableTeamParts Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="c5f74-103">clonableTeamParts enum type</span></span>

> <span data-ttu-id="c5f74-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c5f74-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5f74-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c5f74-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c5f74-106">Beschreibt, welche Teil eines [Team](../resources/team.md) geklont werden soll.</span><span class="sxs-lookup"><span data-stu-id="c5f74-106">Describes which part of a [team](../resources/team.md) should be cloned.</span></span> 

## <a name="members"></a><span data-ttu-id="c5f74-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="c5f74-107">Members</span></span>

| <span data-ttu-id="c5f74-108">Element</span><span class="sxs-lookup"><span data-stu-id="c5f74-108">Member</span></span> | <span data-ttu-id="c5f74-109">Wert</span><span class="sxs-lookup"><span data-stu-id="c5f74-109">Value</span></span>| <span data-ttu-id="c5f74-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5f74-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c5f74-111">Apps</span><span class="sxs-lookup"><span data-stu-id="c5f74-111">apps</span></span>|<span data-ttu-id="c5f74-112">1</span><span class="sxs-lookup"><span data-stu-id="c5f74-112">1</span></span>|<span data-ttu-id="c5f74-113">Kopieren Sie die Liste der installierten apps.</span><span class="sxs-lookup"><span data-stu-id="c5f74-113">Copy the list of installed apps.</span></span>|
|<span data-ttu-id="c5f74-114">Registerkarten</span><span class="sxs-lookup"><span data-stu-id="c5f74-114">tabs</span></span>|<span data-ttu-id="c5f74-115">2</span><span class="sxs-lookup"><span data-stu-id="c5f74-115">2</span></span>|<span data-ttu-id="c5f74-116">die Registerkarten in den Kanälen kopiert.</span><span class="sxs-lookup"><span data-stu-id="c5f74-116">copies the tabs within channels.</span></span>|
|<span data-ttu-id="c5f74-117">settings</span><span class="sxs-lookup"><span data-stu-id="c5f74-117">settings</span></span>|<span data-ttu-id="c5f74-118">4</span><span class="sxs-lookup"><span data-stu-id="c5f74-118">4</span></span>|<span data-ttu-id="c5f74-119">Kopiert alle Einstellungen im Team, zusammen mit den wichtigsten gruppeneinstellungen.</span><span class="sxs-lookup"><span data-stu-id="c5f74-119">Copies all settings within the team, along with key group settings.</span></span>|
|<span data-ttu-id="c5f74-120">Kanäle</span><span class="sxs-lookup"><span data-stu-id="c5f74-120">channels</span></span>|<span data-ttu-id="c5f74-121">8</span><span class="sxs-lookup"><span data-stu-id="c5f74-121">8</span></span>|<span data-ttu-id="c5f74-122">kopiert die Struktur DDE-Kanal (jedoch nicht die Nachrichten im Kanal).</span><span class="sxs-lookup"><span data-stu-id="c5f74-122">copies the channel structure (but not the messages in the channel).</span></span>|
|<span data-ttu-id="c5f74-123">Elemente</span><span class="sxs-lookup"><span data-stu-id="c5f74-123">members</span></span>|<span data-ttu-id="c5f74-124">16</span><span class="sxs-lookup"><span data-stu-id="c5f74-124">16</span></span>|<span data-ttu-id="c5f74-125">kopiert die Elemente und Besitzer des Teams.</span><span class="sxs-lookup"><span data-stu-id="c5f74-125">copies the members and owners of the team.</span></span>|
