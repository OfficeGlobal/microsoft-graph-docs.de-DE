---
title: Teilnehmerliste Ressourcentyp
description: Der Typ Teilnehmer.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: c125589506dbd529d2b45df4171e9d54b346cbba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869832"
---
# <a name="participant-resource-type"></a><span data-ttu-id="77b02-103">Teilnehmerliste Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="77b02-103">participant resource type</span></span>

> <span data-ttu-id="77b02-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="77b02-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77b02-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77b02-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="77b02-106">Der Typ Teilnehmer.</span><span class="sxs-lookup"><span data-stu-id="77b02-106">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="77b02-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="77b02-107">Methods</span></span>

| <span data-ttu-id="77b02-108">Methode</span><span class="sxs-lookup"><span data-stu-id="77b02-108">Method</span></span>                                                          | <span data-ttu-id="77b02-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="77b02-109">Return Type</span></span>                              | <span data-ttu-id="77b02-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77b02-110">Description</span></span>                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [<span data-ttu-id="77b02-111">Abrufen der Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="77b02-111">Get participant</span></span>](../api/participant-get.md)                    | [<span data-ttu-id="77b02-112">Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="77b02-112">participant</span></span>](participant.md)            | <span data-ttu-id="77b02-113">Lesen Sie die Eigenschaften des **Teilnehmers** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="77b02-113">Read properties of the **participant** object.</span></span>    |
| [<span data-ttu-id="77b02-114">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="77b02-114">ConfigureMixer</span></span>](../api/participant-configuremixer.md)          | [<span data-ttu-id="77b02-115">commsOperation</span><span class="sxs-lookup"><span data-stu-id="77b02-115">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="77b02-116">Konfigurieren Sie den Teilnehmerliste Audiomixer.</span><span class="sxs-lookup"><span data-stu-id="77b02-116">Configure the participant audio mixer.</span></span>            |
| [<span data-ttu-id="77b02-117">Einladen</span><span class="sxs-lookup"><span data-stu-id="77b02-117">Invite</span></span>](../api/participant-invite.md)                          | [<span data-ttu-id="77b02-118">commsOperation</span><span class="sxs-lookup"><span data-stu-id="77b02-118">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="77b02-119">Einladen eines Teilnehmers zu den Anruf.</span><span class="sxs-lookup"><span data-stu-id="77b02-119">Invite a participant to the call.</span></span>                 |
| [<span data-ttu-id="77b02-120">Stummschalten von Teilnehmern</span><span class="sxs-lookup"><span data-stu-id="77b02-120">Mute participant</span></span>](../api/participant-mute.md)                  | [<span data-ttu-id="77b02-121">commsOperation</span><span class="sxs-lookup"><span data-stu-id="77b02-121">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="77b02-122">Stummschalten eines Teilnehmers im Gespräch.</span><span class="sxs-lookup"><span data-stu-id="77b02-122">Mute a participant in a call.</span></span>                     |
| [<span data-ttu-id="77b02-123">Stummschalten Sie aller Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="77b02-123">Mute all participants</span></span>](../api/participant-muteall.md)          | [<span data-ttu-id="77b02-124">commsOperation</span><span class="sxs-lookup"><span data-stu-id="77b02-124">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="77b02-125">Stummschalten Sie aller Teilnehmer an der Besprechung.</span><span class="sxs-lookup"><span data-stu-id="77b02-125">Mute all the participants in the meeting.</span></span>         |

## <a name="properties"></a><span data-ttu-id="77b02-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="77b02-126">Properties</span></span>

| <span data-ttu-id="77b02-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77b02-127">Property</span></span>             | <span data-ttu-id="77b02-128">Typ</span><span class="sxs-lookup"><span data-stu-id="77b02-128">Type</span></span>                                     | <span data-ttu-id="77b02-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77b02-129">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="77b02-130">id</span><span class="sxs-lookup"><span data-stu-id="77b02-130">id</span></span>                   | <span data-ttu-id="77b02-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77b02-131">String</span></span>                                   | <span data-ttu-id="77b02-132">Die Teilnehmer-Id.</span><span class="sxs-lookup"><span data-stu-id="77b02-132">The participant id.</span></span>                                          |
| <span data-ttu-id="77b02-133">Info</span><span class="sxs-lookup"><span data-stu-id="77b02-133">info</span></span>                 | [<span data-ttu-id="77b02-134">participantInfo</span><span class="sxs-lookup"><span data-stu-id="77b02-134">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="77b02-135">Die Teilnehmer des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="77b02-135">The participant of the participant.</span></span>                          |
| <span data-ttu-id="77b02-136">isInLobby</span><span class="sxs-lookup"><span data-stu-id="77b02-136">isInLobby</span></span>            | <span data-ttu-id="77b02-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="77b02-137">boolean</span></span>                                  | <span data-ttu-id="77b02-138">True, wenn der Teilnehmer in der Lobby ist</span><span class="sxs-lookup"><span data-stu-id="77b02-138">true if the participant is in lobby</span></span>                          |
| <span data-ttu-id="77b02-139">isMuted</span><span class="sxs-lookup"><span data-stu-id="77b02-139">isMuted</span></span>              | <span data-ttu-id="77b02-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="77b02-140">boolean</span></span>                                  | <span data-ttu-id="77b02-141">True, wenn der Teilnehmer stumm geschaltet ist (Client oder Server stumm geschaltet)</span><span class="sxs-lookup"><span data-stu-id="77b02-141">true if the participant is muted (client or server muted)</span></span>    |
| <span data-ttu-id="77b02-142">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="77b02-142">mediaStreams</span></span>         | <span data-ttu-id="77b02-143">[MediaStream](mediastream.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="77b02-143">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="77b02-144">Die Liste der Mediendatenströme.</span><span class="sxs-lookup"><span data-stu-id="77b02-144">The list of media streams.</span></span>                                   |
| <span data-ttu-id="77b02-145">Metadaten</span><span class="sxs-lookup"><span data-stu-id="77b02-145">metadata</span></span>             | <span data-ttu-id="77b02-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77b02-146">String</span></span>                                   | <span data-ttu-id="77b02-147">Blob-Daten von den Teilnehmer in der Teilnehmerliste einer</span><span class="sxs-lookup"><span data-stu-id="77b02-147">A blob of data provided by the participant in the roster</span></span>     |
| <span data-ttu-id="77b02-148">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="77b02-148">recordingInfo</span></span>        | [<span data-ttu-id="77b02-149">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="77b02-149">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="77b02-150">Informationen zu gibt an, ob der Teilnehmer Aufzeichnung Funktionalität verfügt.</span><span class="sxs-lookup"><span data-stu-id="77b02-150">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="77b02-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="77b02-151">Relationships</span></span>
<span data-ttu-id="77b02-152">Keine</span><span class="sxs-lookup"><span data-stu-id="77b02-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77b02-153">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="77b02-153">JSON representation</span></span>

<span data-ttu-id="77b02-154">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="77b02-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "String (identifier)",
  "info": {"@odata.type": "#microsoft.graph.participantInfo"},
  "isInLobby": true,
  "isMuted": true,
  "mediaStreams": [ { "@odata.type": "#microsoft.graph.mediaStream" } ],
  "metadata": "String",
  "recordingInfo": { "@odata.type": "#microsoft.graph.recordingInfo" }
}
```

## <a name="example"></a><span data-ttu-id="77b02-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="77b02-155">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "info": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "en-US",
    "region": "westus"
  },
  "isInLobby": false,
  "isMuted": false,
  "mediaStreams": [
    {
      "sourceId": "1",
      "direction": "sendReceive",
      "label": "main-audio",
      "mediaType": "audio",
      "serverMuted": false
    }
  ],
  "metadata": "metadata-value",
  "recordingInfo": {
    "status": "recordingCapable"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
