---
title: Teilnehmerliste Ressourcentyp
description: Der Typ Teilnehmer.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f49526824b2b6c4eb4a5065f05ab4c765d299faa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508146"
---
# <a name="participant-resource-type"></a><span data-ttu-id="27834-103">Teilnehmerliste Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="27834-103">participant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27834-104">Der Typ Teilnehmer.</span><span class="sxs-lookup"><span data-stu-id="27834-104">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="27834-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="27834-105">Methods</span></span>

| <span data-ttu-id="27834-106">Methode</span><span class="sxs-lookup"><span data-stu-id="27834-106">Method</span></span>                                                          | <span data-ttu-id="27834-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="27834-107">Return Type</span></span>                              | <span data-ttu-id="27834-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27834-108">Description</span></span>                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [<span data-ttu-id="27834-109">Abrufen der Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="27834-109">Get participant</span></span>](../api/participant-get.md)                    | [<span data-ttu-id="27834-110">Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="27834-110">participant</span></span>](participant.md)            | <span data-ttu-id="27834-111">Lesen Sie die Eigenschaften des **Teilnehmers** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="27834-111">Read properties of the **participant** object.</span></span>    |
| [<span data-ttu-id="27834-112">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="27834-112">ConfigureMixer</span></span>](../api/participant-configuremixer.md)          | [<span data-ttu-id="27834-113">commsOperation</span><span class="sxs-lookup"><span data-stu-id="27834-113">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="27834-114">Konfigurieren Sie den Teilnehmerliste Audiomixer.</span><span class="sxs-lookup"><span data-stu-id="27834-114">Configure the participant audio mixer.</span></span>            |
| [<span data-ttu-id="27834-115">Einladen</span><span class="sxs-lookup"><span data-stu-id="27834-115">Invite</span></span>](../api/participant-invite.md)                          | [<span data-ttu-id="27834-116">commsOperation</span><span class="sxs-lookup"><span data-stu-id="27834-116">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="27834-117">Einladen eines Teilnehmers zu den Anruf.</span><span class="sxs-lookup"><span data-stu-id="27834-117">Invite a participant to the call.</span></span>                 |
| [<span data-ttu-id="27834-118">Stummschalten von Teilnehmern</span><span class="sxs-lookup"><span data-stu-id="27834-118">Mute participant</span></span>](../api/participant-mute.md)                  | [<span data-ttu-id="27834-119">commsOperation</span><span class="sxs-lookup"><span data-stu-id="27834-119">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="27834-120">Stummschalten eines Teilnehmers im Gespräch.</span><span class="sxs-lookup"><span data-stu-id="27834-120">Mute a participant in a call.</span></span>                     |
| [<span data-ttu-id="27834-121">Stummschalten Sie aller Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="27834-121">Mute all participants</span></span>](../api/participant-muteall.md)          | [<span data-ttu-id="27834-122">commsOperation</span><span class="sxs-lookup"><span data-stu-id="27834-122">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="27834-123">Stummschalten Sie aller Teilnehmer an der Besprechung.</span><span class="sxs-lookup"><span data-stu-id="27834-123">Mute all the participants in the meeting.</span></span>         |

## <a name="properties"></a><span data-ttu-id="27834-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="27834-124">Properties</span></span>

| <span data-ttu-id="27834-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="27834-125">Property</span></span>             | <span data-ttu-id="27834-126">Typ</span><span class="sxs-lookup"><span data-stu-id="27834-126">Type</span></span>                                     | <span data-ttu-id="27834-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27834-127">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="27834-128">id</span><span class="sxs-lookup"><span data-stu-id="27834-128">id</span></span>                   | <span data-ttu-id="27834-129">String</span><span class="sxs-lookup"><span data-stu-id="27834-129">String</span></span>                                   | <span data-ttu-id="27834-130">Die Teilnehmer-Id.</span><span class="sxs-lookup"><span data-stu-id="27834-130">The participant id.</span></span>                                          |
| <span data-ttu-id="27834-131">Info</span><span class="sxs-lookup"><span data-stu-id="27834-131">info</span></span>                 | [<span data-ttu-id="27834-132">participantInfo</span><span class="sxs-lookup"><span data-stu-id="27834-132">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="27834-133">Die Teilnehmer des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="27834-133">The participant of the participant.</span></span>                          |
| <span data-ttu-id="27834-134">isInLobby</span><span class="sxs-lookup"><span data-stu-id="27834-134">isInLobby</span></span>            | <span data-ttu-id="27834-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="27834-135">boolean</span></span>                                  | <span data-ttu-id="27834-136">True, wenn der Teilnehmer in der Lobby ist</span><span class="sxs-lookup"><span data-stu-id="27834-136">true if the participant is in lobby</span></span>                          |
| <span data-ttu-id="27834-137">isMuted</span><span class="sxs-lookup"><span data-stu-id="27834-137">isMuted</span></span>              | <span data-ttu-id="27834-138">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="27834-138">boolean</span></span>                                  | <span data-ttu-id="27834-139">True, wenn der Teilnehmer stumm geschaltet ist (Client oder Server stumm geschaltet)</span><span class="sxs-lookup"><span data-stu-id="27834-139">true if the participant is muted (client or server muted)</span></span>    |
| <span data-ttu-id="27834-140">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="27834-140">mediaStreams</span></span>         | <span data-ttu-id="27834-141">[MediaStream](mediastream.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="27834-141">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="27834-142">Die Liste der Mediendatenströme.</span><span class="sxs-lookup"><span data-stu-id="27834-142">The list of media streams.</span></span>                                   |
| <span data-ttu-id="27834-143">$metadata</span><span class="sxs-lookup"><span data-stu-id="27834-143">metadata</span></span>             | <span data-ttu-id="27834-144">String</span><span class="sxs-lookup"><span data-stu-id="27834-144">String</span></span>                                   | <span data-ttu-id="27834-145">Blob-Daten von den Teilnehmer in der Teilnehmerliste einer</span><span class="sxs-lookup"><span data-stu-id="27834-145">A blob of data provided by the participant in the roster</span></span>     |
| <span data-ttu-id="27834-146">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="27834-146">recordingInfo</span></span>        | [<span data-ttu-id="27834-147">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="27834-147">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="27834-148">Informationen zu gibt an, ob der Teilnehmer Aufzeichnung Funktionalität verfügt.</span><span class="sxs-lookup"><span data-stu-id="27834-148">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="27834-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="27834-149">Relationships</span></span>
<span data-ttu-id="27834-150">Keine</span><span class="sxs-lookup"><span data-stu-id="27834-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27834-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="27834-151">JSON representation</span></span>

<span data-ttu-id="27834-152">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="27834-152">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="27834-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="27834-153">Example</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/participant.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
