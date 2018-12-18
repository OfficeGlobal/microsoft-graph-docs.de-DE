---
title: Abrufen von unveränderlichen Bezeichnern für Outlook-Ressourcen
description: 'Outlook-Elemente (Nachrichten, Ereignisse, Kontakte, Aufgaben) haben ein interessantes Verhalten, das Sie vermutlich entweder noch nie bemerkt haben oder das bei Ihnen erhebliche Frustration ausgelöst hat: ihre IDs ändern sich. Das geschieht nicht oft, nur wenn das Element verschoben wird, es kann aber für Apps, die IDs zwecks späterer Verwendung offline speichern, zu echten Problemen führen. Unveränderliche Bezeichner ermöglichen Ihrer Anwendung das Abrufen einer ID, die sich über die gesamte Lebensdauer des Elements nicht ändert.'
author: angelgolfer-ms
ms.openlocfilehash: 34d88ed2cbc39902f1240757367beb112cc007b4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315197"
---
# <a name="get-immutable-identifiers-for-outlook-resources"></a><span data-ttu-id="f7c53-105">Abrufen von unveränderlichen Bezeichnern für Outlook-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="f7c53-105">Get immutable identifiers for Outlook resources</span></span>

<span data-ttu-id="f7c53-106">Outlook-Elemente (Nachrichten, Ereignisse, Kontakte, Aufgaben) haben ein interessantes Verhalten, das Sie vermutlich entweder noch nie bemerkt haben oder das bei Ihnen erhebliche Frustration ausgelöst hat: ihre IDs ändern sich.</span><span class="sxs-lookup"><span data-stu-id="f7c53-106">Outlook items (messages, events, contacts, tasks) have an interesting behavior that you've probably either never noticed or has caused you significant frustration: their IDs change.</span></span> <span data-ttu-id="f7c53-107">Das geschieht nicht oft, nur wenn das Element verschoben wird, es kann aber für Apps, die IDs zwecks späterer Verwendung offline speichern, zu echten Problemen führen.</span><span class="sxs-lookup"><span data-stu-id="f7c53-107">It doesn't happen often, only if the item is moved, but it can cause real problems for apps that store IDs offline for later use.</span></span> <span data-ttu-id="f7c53-108">Unveränderliche Bezeichner ermöglichen Ihrer Anwendung das Abrufen einer ID, die sich über die gesamte Lebensdauer des Elements nicht ändert.</span><span class="sxs-lookup"><span data-stu-id="f7c53-108">Immutable identifiers enables your application to obtain an ID that does not change for the lifetime of the item.</span></span>

> <span data-ttu-id="f7c53-109">**Wichtig:** Unveränderliche Bezeichner sind nur in der /beta-Version von Microsoft Graph verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f7c53-109">**Important:** Immutable identifiers are only avaiable on the /beta version in Microsoft Graph.</span></span>

## <a name="how-it-works"></a><span data-ttu-id="f7c53-110">Funktionsweise</span><span class="sxs-lookup"><span data-stu-id="f7c53-110">How it works</span></span>

<span data-ttu-id="f7c53-111">Unveränderliche IDs stellen ein optionales Feature von Microsoft Graph dar.</span><span class="sxs-lookup"><span data-stu-id="f7c53-111">Immutable ID is an optional feature for Microsoft Graph.</span></span> <span data-ttu-id="f7c53-112">Um sich dafür zu entscheiden, muss Ihre Anwendung einen zusätzlichen HTTP-Header in Ihren API-Anforderungen senden:</span><span class="sxs-lookup"><span data-stu-id="f7c53-112">To opt in, your application needs to send an additional HTTP header in your API requests:</span></span>

```http
Prefer: IdType="ImmutableId"
```

<span data-ttu-id="f7c53-113">Dieser Header gilt nur für die Anforderung, in der er enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="f7c53-113">This header only applies to the request it is included with.</span></span> <span data-ttu-id="f7c53-114">Wenn Sie immer unveränderliche IDs verwenden möchten, müssen Sie diesen Header in jede API-Anforderung aufnehmen.</span><span class="sxs-lookup"><span data-stu-id="f7c53-114">If you want to always use immutable IDs, you must include this header with every API request.</span></span>

## <a name="lifetime-of-immutable-ids"></a><span data-ttu-id="f7c53-115">Lebensdauer unveränderlicher IDs</span><span class="sxs-lookup"><span data-stu-id="f7c53-115">Lifetime of Immutable IDs</span></span>

<span data-ttu-id="f7c53-116">Die unveränderliche ID eines Elements ändert sich nicht, solange das Element im gleichen Postfach verbleibt.</span><span class="sxs-lookup"><span data-stu-id="f7c53-116">An item's immutable ID will not change so long as the item stays in the same mailbox.</span></span> <span data-ttu-id="f7c53-117">Das bedeutet, dass sich die unveränderliche ID NICHT ändert, wenn das Element in einen anderen Ordner im Postfach verschoben wird.</span><span class="sxs-lookup"><span data-stu-id="f7c53-117">That means that immutable ID will NOT change if the item is moved to a different folder in the mailbox.</span></span> <span data-ttu-id="f7c53-118">Die unveränderliche ID ändert sich aber unter diesen Umständen:</span><span class="sxs-lookup"><span data-stu-id="f7c53-118">However, the immutable ID will change if:</span></span>

- <span data-ttu-id="f7c53-119">Der Benutzer verschiebt das Element in ein Archivpostfach</span><span class="sxs-lookup"><span data-stu-id="f7c53-119">The user moves the item to an archive mailbox</span></span>
- <span data-ttu-id="f7c53-120">Der Benutzer exportiert das Element (in eine PST-Datei, als MSG-Datei usw.) und importiert es anschließend wieder in sein Postfach</span><span class="sxs-lookup"><span data-stu-id="f7c53-120">The user exports the item (to a PST, as an MSG file, etc.) and re-imports it into their mailbox</span></span>

## <a name="items-that-support-immutable-id"></a><span data-ttu-id="f7c53-121">Elemente, die unveränderliche IDs unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f7c53-121">Items that support immutable ID</span></span>

<span data-ttu-id="f7c53-122">Die folgenden Elemente unterstützen unveränderliche IDs:</span><span class="sxs-lookup"><span data-stu-id="f7c53-122">The following items support immutable IDs:</span></span>

- [<span data-ttu-id="f7c53-123">Ressourcentyp Nachricht</span><span class="sxs-lookup"><span data-stu-id="f7c53-123">message resource type</span></span>](/graph/api/resources/message?view=graph-rest-beta)
- [<span data-ttu-id="f7c53-124">Ressourcentyp Anlage</span><span class="sxs-lookup"><span data-stu-id="f7c53-124">attachment resource type</span></span>](/graph/api/resources/attachment?view=graph-rest-beta)
- [<span data-ttu-id="f7c53-125">Ressourcentyp Ereignis</span><span class="sxs-lookup"><span data-stu-id="f7c53-125">event resource type</span></span>](/graph/api/resources/event?view=graph-rest-beta)
- [<span data-ttu-id="f7c53-126">Ressourcentyp eventMessage</span><span class="sxs-lookup"><span data-stu-id="f7c53-126">eventMessage resource type</span></span>](/graph/api/resources/eventmessage?view=graph-rest-beta)
- [<span data-ttu-id="f7c53-127">Ressourcentyp Kontakt</span><span class="sxs-lookup"><span data-stu-id="f7c53-127">contact resource type</span></span>](/graph/api/resources/contact?view=graph-rest-beta)
- [<span data-ttu-id="f7c53-128">Ressourcentyp outlookTask</span><span class="sxs-lookup"><span data-stu-id="f7c53-128">outlookTask resource type</span></span>](/graph/api/resources/outlooktask?view=graph-rest-beta)

<span data-ttu-id="f7c53-129">Containertypen (mailFolder, calendar usw.) unterstützen keine unveränderlichen IDs, aber ihre regulären IDs stellen bereits Konstanten dar.</span><span class="sxs-lookup"><span data-stu-id="f7c53-129">Container types (mailFolder, calendar, etc.) do not support immutable ID, but their regular IDs were already constant.</span></span>

## <a name="immutable-id-with-change-notifications"></a><span data-ttu-id="f7c53-130">Unveränderliche IDs mit Änderungsbenachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="f7c53-130">Immutable ID with change notifications</span></span>

<span data-ttu-id="f7c53-131">Sie können festlegen, dass Microsoft Graph unveränderliche IDs in Änderungsbenachrichtigungen sendet, indem Sie den Header `Prefer: IdType="ImmutableId"` beim [Erstellen eines Abonnements](/graph/api/subscription-post-subscriptions?view=graph-rest-beta) einschließen.</span><span class="sxs-lookup"><span data-stu-id="f7c53-131">You can request that Microsoft Graph send immutable IDs in change notifications by including the `Prefer: IdType="ImmutableId"` header when [creating a subscription](/graph/api/subscription-post-subscriptions?view=graph-rest-beta).</span></span> <span data-ttu-id="f7c53-132">Vorhandene Abonnements, die ohne den Header erstellt wurden, verwenden weiterhin das ID-Standardformat.</span><span class="sxs-lookup"><span data-stu-id="f7c53-132">Existing subscriptions created without the header will continue to use the default ID format.</span></span> <span data-ttu-id="f7c53-133">Um vorhandene IDs auf die Verwendung von unveränderlichen IDs umzustellen, müssen Sie sie löschen und unter Verwendung des Headers neu erstellen.</span><span class="sxs-lookup"><span data-stu-id="f7c53-133">In order to switch existing subscriptions to use immutable IDs, you must delete and recreate them using the header.</span></span>

## <a name="immutable-id-with-delta-query"></a><span data-ttu-id="f7c53-134">Unveränderliche IDs mit Delta-Abfragen</span><span class="sxs-lookup"><span data-stu-id="f7c53-134">Immutable ID with delta query</span></span>

<span data-ttu-id="f7c53-135">Sie können festlegen, dass Microsoft Graph für unterstützte Ressourcentypen unveränderliche IDs in [Antworten auf Delta-Abfragen](delta-query-overview.md) zurückgibt, indem Sie den Header `Prefer: IdType="ImmutableId"` einschließen.</span><span class="sxs-lookup"><span data-stu-id="f7c53-135">You can request that Microsoft Graph return immutable IDs in [delta query responses](delta-query-overview.md) for supported resource types by including the `Prefer: IdType="ImmutableId"` header.</span></span> <span data-ttu-id="f7c53-136">Die von Delta-Abfragen zurückgegebenen Werte `nextLink` und `deltaLink` sind mit beiden ID-Formaten kompatibel, daher muss Ihre Anwendung nicht neu synchronisiert werden, um unveränderliche IDs zu nutzen.</span><span class="sxs-lookup"><span data-stu-id="f7c53-136">The `nextLink` and `deltaLink` values returned by delta queries are compatible with both ID formats, so your application does not need to re-synchronize to take advantage of immutable ID.</span></span> <span data-ttu-id="f7c53-137">Sie können den Header verwenden, um von jetzt an unveränderliche IDs abzurufen, und Sie können [den Speicher Ihrer App](#updating-existing-data) separat aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="f7c53-137">You can use the header to get immutable IDs going forward, and you can [update your app's storage](#updating-existing-data) separately.</span></span>

## <a name="updating-existing-data"></a><span data-ttu-id="f7c53-138">Aktualisieren vorhandener Daten</span><span class="sxs-lookup"><span data-stu-id="f7c53-138">Updating existing data</span></span>

<span data-ttu-id="f7c53-139">Wenn Sie bereits über eine Datenbank verfügen, die mit Tausenden regulärer IDs gefüllt ist, können Sie diese IDs mithilfe der Funktion [translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-beta) in das unveränderliche Format konvertieren.</span><span class="sxs-lookup"><span data-stu-id="f7c53-139">If you've already got a database filled with thousands of regular IDs, you can migrate those IDs to immutable format using the [translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-beta) function.</span></span> <span data-ttu-id="f7c53-140">Sie können ein Array von bis zu 1.000 IDs angeben, die in ein Zielformat übersetzt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f7c53-140">You can provide an array of up to 1000 IDs to be translated into a target format.</span></span>

> <span data-ttu-id="f7c53-141">**Hinweis:** `translateExchangeIds` kann auch für die Migration von Exchange-Webdiensten nach Microsoft Graph verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="f7c53-141">**Note:** You can also use `translateExchangeIds` to migrate Exchange Web Services applications to Microsoft Graph.</span></span>

### <a name="example"></a><span data-ttu-id="f7c53-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f7c53-142">Example</span></span>

<span data-ttu-id="f7c53-143">Im folgenden Beispiel wird eine normale Graph-ID in eine unveränderliche Graph-ID übersetzt.</span><span class="sxs-lookup"><span data-stu-id="f7c53-143">The following example translates a normal Graph ID to an immutable Graph ID.</span></span>

#### <a name="request"></a><span data-ttu-id="f7c53-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7c53-144">Request</span></span>

```http
POST https://graph.microsoft.com/beta/me/translateExchangeIds

{
  "inputIds" :
  [
    "AQMkAGM2…"
  ],
  "targetIdType" : "restImmutableEntryId",
  "sourceIdType" : "restId"
}
```

#### <a name="response"></a><span data-ttu-id="f7c53-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7c53-145">Response</span></span>

```http
HTTP 200 OK

{
  "value": [
    {
      "targetId": "AAkALgAA...",
      "sourceId": "AQMkAGM2..."
    }
  ]
}
```