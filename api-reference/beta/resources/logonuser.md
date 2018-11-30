---
title: LogonUser Ressourcentyp
description: Enthält Statusinformationen zu der angemeldete Benutzer auf diesem host
ms.openlocfilehash: 80ff69453e99f5cd5103f85cd7d8c45696057f7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065124"
---
# <a name="logonuser-resource-type"></a><span data-ttu-id="454ca-103">LogonUser Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="454ca-103">logonUser resource type</span></span>

<span data-ttu-id="454ca-104">Enthält Statusinformationen zu der angemeldete Benutzer auf diesem host</span><span class="sxs-lookup"><span data-stu-id="454ca-104">Contains stateful information about the logged on user on this host</span></span>

## <a name="properties"></a><span data-ttu-id="454ca-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="454ca-105">Properties</span></span>

| <span data-ttu-id="454ca-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="454ca-106">Property</span></span>   | <span data-ttu-id="454ca-107">Typ</span><span class="sxs-lookup"><span data-stu-id="454ca-107">Type</span></span> |<span data-ttu-id="454ca-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="454ca-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="454ca-109">accountDomain</span><span class="sxs-lookup"><span data-stu-id="454ca-109">accountDomain</span></span>|<span data-ttu-id="454ca-110">String</span><span class="sxs-lookup"><span data-stu-id="454ca-110">String</span></span>|<span data-ttu-id="454ca-111">Domäne des Benutzerkontos verwendet für die Anmeldung.</span><span class="sxs-lookup"><span data-stu-id="454ca-111">Domain of user account used to logon.</span></span>|
|<span data-ttu-id="454ca-112">accountName</span><span class="sxs-lookup"><span data-stu-id="454ca-112">accountName</span></span>|<span data-ttu-id="454ca-113">String</span><span class="sxs-lookup"><span data-stu-id="454ca-113">String</span></span>|<span data-ttu-id="454ca-114">Kontoname des verwendete Benutzerkonto für die Anmeldung.</span><span class="sxs-lookup"><span data-stu-id="454ca-114">Account name of user account used to logon.</span></span>|
|<span data-ttu-id="454ca-115">accountType</span><span class="sxs-lookup"><span data-stu-id="454ca-115">accountType</span></span>|<span data-ttu-id="454ca-116">String</span><span class="sxs-lookup"><span data-stu-id="454ca-116">String</span></span>|<span data-ttu-id="454ca-117">Benutzerkontotyp pro Windows-Definition.</span><span class="sxs-lookup"><span data-stu-id="454ca-117">User Account type, per Windows definition.</span></span> <span data-ttu-id="454ca-118">Mögliche Werte: sind `unknown`, `standard`, `power` und `administrator`.</span><span class="sxs-lookup"><span data-stu-id="454ca-118">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="454ca-119">firstSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="454ca-119">firstSeenDateTime</span></span>|<span data-ttu-id="454ca-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="454ca-120">DateTimeOffset</span></span>|<span data-ttu-id="454ca-121">DateTime, an dem die früheste Anmeldung durch dieses Benutzerkonto stattgefunden hat (Punkt Anbieter bestimmt).</span><span class="sxs-lookup"><span data-stu-id="454ca-121">DateTime at which the earliest logon by this user account occurred (provider-determined period).</span></span> <span data-ttu-id="454ca-122">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="454ca-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="454ca-123">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="454ca-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="454ca-124">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="454ca-124">lastSeenDateTime</span></span>|<span data-ttu-id="454ca-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="454ca-125">DateTimeOffset</span></span>|<span data-ttu-id="454ca-126">DateTime, an dem die aktuelle Anmeldung durch dieses Benutzerkonto aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="454ca-126">DateTime at which the latest logon by this user account occurred.</span></span> <span data-ttu-id="454ca-127">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="454ca-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="454ca-128">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="454ca-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="454ca-129">logonId</span><span class="sxs-lookup"><span data-stu-id="454ca-129">logonId</span></span>|<span data-ttu-id="454ca-130">String</span><span class="sxs-lookup"><span data-stu-id="454ca-130">String</span></span>|<span data-ttu-id="454ca-131">Benutzer-Anmelde-ID</span><span class="sxs-lookup"><span data-stu-id="454ca-131">User logon ID.</span></span>|
|<span data-ttu-id="454ca-132">logonTypes</span><span class="sxs-lookup"><span data-stu-id="454ca-132">logonTypes</span></span>|<span data-ttu-id="454ca-133">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="454ca-133">String collection</span></span>|<span data-ttu-id="454ca-134">Auflistung der Anmeldetypen beobachtet aus der angemeldete Benutzer beim ersten bis zum letzten angezeigt.</span><span class="sxs-lookup"><span data-stu-id="454ca-134">Collection of the logon types observed for the logged on user from when first to last seen.</span></span> <span data-ttu-id="454ca-135">Mögliche Werte sind: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch` und `service`.</span><span class="sxs-lookup"><span data-stu-id="454ca-135">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="454ca-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="454ca-136">JSON representation</span></span>

<span data-ttu-id="454ca-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="454ca-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.logonUser"
}-->

```json
{
  "accountDomain": "String",
  "accountName": "String",
  "accountType": "String",
  "firstSeenDateTime": "String (timestamp)",
  "lastSeenDateTime": "String (timestamp)",
  "logonId": "String",
  "logonTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "logonUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->