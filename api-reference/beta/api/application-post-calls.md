---
title: Erstellen von Anrufen
description: Erstellen Sie einen neuen Anruf.
author: VinodRavichandran
ms.openlocfilehash: a2d34ccf3d77d165b8a92114353d5f6cb8bed674
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380387"
---
# <a name="create-call"></a><span data-ttu-id="07418-103">Erstellen von Anrufen</span><span class="sxs-lookup"><span data-stu-id="07418-103">Create call</span></span>

> <span data-ttu-id="07418-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="07418-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07418-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="07418-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07418-106">Erstellen Sie einen neuen Anruf.</span><span class="sxs-lookup"><span data-stu-id="07418-106">Create a new call.</span></span>

## <a name="permissions"></a><span data-ttu-id="07418-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="07418-107">Permissions</span></span>
<span data-ttu-id="07418-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07418-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="07418-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="07418-110">Permission type</span></span>                        | <span data-ttu-id="07418-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="07418-111">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="07418-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="07418-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="07418-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="07418-113">Not Supported</span></span>                                                                           |
| <span data-ttu-id="07418-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="07418-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07418-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="07418-115">Not Supported</span></span>                                                                           |
| <span data-ttu-id="07418-116">Application</span><span class="sxs-lookup"><span data-stu-id="07418-116">Application</span></span>                            | <span data-ttu-id="07418-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="07418-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="07418-118">**Hinweis:** Für einen Anruf mit Medien app gehostet wird benötigen Sie die Berechtigung Calls.AccessMedia.All mit einem der in der vorherigen Tabelle aufgelisteten Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="07418-118">**Note:** For a call with app hosted media, you need the Calls.AccessMedia.All permission with one of the permissions listed in the previous table.</span></span>

## <a name="http-request"></a><span data-ttu-id="07418-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="07418-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls
POST /applications/{id}/calls
```

## <a name="request-headers"></a><span data-ttu-id="07418-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="07418-120">Request headers</span></span>
| <span data-ttu-id="07418-121">Name</span><span class="sxs-lookup"><span data-stu-id="07418-121">Name</span></span>          | <span data-ttu-id="07418-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07418-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="07418-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="07418-123">Authorization</span></span> | <span data-ttu-id="07418-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="07418-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07418-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="07418-126">Request body</span></span>
<span data-ttu-id="07418-127">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines Objekts [aufrufen](../resources/call.md) .</span><span class="sxs-lookup"><span data-stu-id="07418-127">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

> <span data-ttu-id="07418-128">**Hinweis:** Eigenschaften als markiert `Server generated` werden ignoriert, bei der Verarbeitung von `POST` auf `app/calls`.</span><span class="sxs-lookup"><span data-stu-id="07418-128">**Note:** Properties marked as `Server generated` are ignored when processing `POST` on `app/calls`.</span></span>

## <a name="response"></a><span data-ttu-id="07418-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="07418-129">Response</span></span>
<span data-ttu-id="07418-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines Objekts [aufrufen,](../resources/call.md) in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="07418-130">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="07418-131">Beispiele</span><span class="sxs-lookup"><span data-stu-id="07418-131">Examples</span></span>

### <a name="create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="07418-132">Erstellen Sie Peer-zu-Peer-VOIP-Anruf mit gehosteten Dienst Medien</span><span class="sxs-lookup"><span data-stu-id="07418-132">Create peer to peer VOIP call with service hosted media</span></span>

> <span data-ttu-id="07418-133">**Hinweis:** Dieses Anrufs benötigt die Berechtigung Calls.Initiate.All.</span><span class="sxs-lookup"><span data-stu-id="07418-133">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="07418-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="07418-134">Request</span></span>
<span data-ttu-id="07418-135">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="07418-135">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-call-from-application"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json

{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
      {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      {
        "uri": "https://cdn.contoso.com/cool.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
      }
    ]
  },
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "subject": "Test Call",
  "targets": [
    {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      }
    }
  ],
  "tenantId": "tenantId-value"
}
```

##### <a name="response"></a><span data-ttu-id="07418-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="07418-136">Response</span></span>

> <span data-ttu-id="07418-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="07418-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json


{
  "id": "57DAB8B1894C409AB240BD8BEAE78896",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
      {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      {
        "uri": "https://cdn.contoso.com/cool.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
      }
    ]
  },
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "subject": "Test Call",
  "targets": [
    {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      }
    }
  ],
  "tenantId": "tenantId-value"
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="07418-139">Benachrichtigung - Einrichtung</span><span class="sxs-lookup"><span data-stu-id="07418-139">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "state": "establishing",
        "direction": "outgoing"
      }
    }
  ]
}
```
##### <a name="notification---established"></a><span data-ttu-id="07418-140">Benachrichtigung - eingerichtet</span><span class="sxs-lookup"><span data-stu-id="07418-140">Notification - established</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "established"
        }
    }
  ]
}
```

### <a name="create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="07418-141">Erstellen Sie Peer-zu-Peer-VOIP-Anruf mit gehostete Anwendungsmedien</span><span class="sxs-lookup"><span data-stu-id="07418-141">Create peer to peer VOIP call with application hosted media</span></span>

> <span data-ttu-id="07418-142">Hinweis: Muss Berechtigung Calls.Initiate.All und Calls.AccessMedia.All.</span><span class="sxs-lookup"><span data-stu-id="07418-142">Note: Needs Calls.Initiate.All and Calls.AccessMedia.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="07418-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="07418-143">Request</span></span>
<span data-ttu-id="07418-144">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="07418-144">The following example shows the request.</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  },
  "requestedModalities": [ "audio" ],
  "source": {
    "identity": {
      "application": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "IT Bot"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "subject": "Test Call",
  "targets": [
    {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      }
    }
  ],
  "tenantId": "tenantId-value"
}
```

### <a name="create-group-call-with-service-hosted-media"></a><span data-ttu-id="07418-145">Erstellen Sie gruppenanruf mit gehosteten Dienst Medien</span><span class="sxs-lookup"><span data-stu-id="07418-145">Create group call with service hosted media</span></span>

> <span data-ttu-id="07418-146">**Hinweis:** In diesem Beispiel wird erforderlich die Calls.InitiateGroupCalls.All und Calls.AccessMedia.All-Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="07418-146">**Note:** This example needs the Calls.InitiateGroupCalls.All and Calls.AccessMedia.All permissions.</span></span>

##### <a name="request"></a><span data-ttu-id="07418-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="07418-147">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "subject": "Test Call",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    }
  },
  "targets": [
    {
      "identity": {
        "user": {
          "id": "29362BD4-CD58-4ED0-A206-0E4A33DBB0B6",
          "displayName": "Heidi Steen"
        }
      }
    },
    {
      "identity": {
        "phone": {
          "displayName": "+12345678890",
          "id": "+12345678890"
        }
      }
    }
  ],
  "requestedModalities": [ "audio", "video" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
      {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      {
        "uri": "https://cdn.contoso.com/cool.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
      }
    ]
  },
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "0",
    "replyChainMessageId": null
  }
}
```

### <a name="join-private-meeting-with-service-hosted-media"></a><span data-ttu-id="07418-148">Private an Besprechung teilnehmen mit Medien gehosteten Dienst</span><span class="sxs-lookup"><span data-stu-id="07418-148">Join private meeting with service hosted media</span></span>

> <span data-ttu-id="07418-149">**Hinweis:** In diesem Beispiel wird benötigt die Berechtigung Calls.JoinGroupCalls.All.</span><span class="sxs-lookup"><span data-stu-id="07418-149">**Note:** This example needs the Calls.JoinGroupCalls.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="07418-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="07418-150">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "subject": "Test Call",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    }
  },
  "requestedModalities": [ "audio", "video" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
      {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      {
        "uri": "https://cdn.contoso.com/cool.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
      }
    ]
  },
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "0"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
        "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
      }
    }
  }
}
```

### <a name="join-channel-meeting-with-service-hosted-media"></a><span data-ttu-id="07418-151">Teilnehmen an Channel-Besprechung mit Medien gehosteten Dienst</span><span class="sxs-lookup"><span data-stu-id="07418-151">Join channel meeting with service hosted media</span></span>

> <span data-ttu-id="07418-152">**Hinweis:** In diesem Beispiel wird benötigt die Berechtigung Calls.JoinGroupCalls.All.</span><span class="sxs-lookup"><span data-stu-id="07418-152">**Note:** This example needs the Calls.JoinGroupCalls.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="07418-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="07418-153">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "subject": "Test Call",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    }
  },
  "requestedModalities": [ "audio", "video" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
      {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      {
        "uri": "https://cdn.contoso.com/cool.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
      }
    ]
  },
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "1507228578052",
    "replyChainMessageId": null
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
        "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
      }
    }
  }
}
```

### <a name="join-channel-meeting-as-a-guest-with-service-hosted-media"></a><span data-ttu-id="07418-154">Teilnehmen an Channel Besprechung als Gast mit Medien gehosteten Dienst</span><span class="sxs-lookup"><span data-stu-id="07418-154">Join channel meeting as a guest with service hosted media</span></span>

> <span data-ttu-id="07418-155">**Hinweis:** In diesem Beispiel wird benötigt die Berechtigung Calls.JoinGroupCallsAsGuest.All.</span><span class="sxs-lookup"><span data-stu-id="07418-155">**Note:** This example needs the Calls.JoinGroupCallsAsGuest.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="07418-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="07418-156">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```
<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "subject": "Test Call",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "source": {
    "identity": {
      "user": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698",
        "displayName": "App_Guest_DisplayName",
        "identityProvider": "None"
      }
    }
  },
  "requestedModalities": [ "audio", "video" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
      {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      {
        "uri": "https://cdn.contoso.com/cool.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
      }
    ]
  },
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "1507228578052",
    "replyChainMessageId": null
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
        "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
      }
    }
  }
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create call",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
