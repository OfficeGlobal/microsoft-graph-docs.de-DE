---
title: Erstellen Sie und senden Sie eine Benachrichtigung
description: 'Erstellen Sie und senden Sie eine Benachrichtigung für einen Benutzer über Microsoft Graph. Die Benachrichtigung wird in der Microsoft Graph-Benachrichtigung feed Store gespeichert und an alle Geräte-Endpunkten, bei denen der Benutzer, in angemeldet ist allen app-Clients gesendet.  '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 70c7992a6fd323b909d948976132304fa04393c4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528445"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="06573-104">Erstellen Sie und senden Sie eine Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="06573-104">Create and send a notification</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06573-105">Erstellen Sie und senden Sie eine Benachrichtigung für einen Benutzer über Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="06573-105">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="06573-106">Die Benachrichtigung wird in der Microsoft Graph-Benachrichtigung feed Store gespeichert und an alle Geräte-Endpunkten, bei denen der Benutzer, in angemeldet ist allen app-Clients gesendet.</span><span class="sxs-lookup"><span data-stu-id="06573-106">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  
## <a name="permissions"></a><span data-ttu-id="06573-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="06573-107">Permissions</span></span>
<span data-ttu-id="06573-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06573-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06573-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="06573-110">Permission type</span></span>      | <span data-ttu-id="06573-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="06573-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06573-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="06573-112">Delegated (work or school account)</span></span> | <span data-ttu-id="06573-113">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="06573-113">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="06573-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="06573-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06573-115">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="06573-115">Notifications.ReadWrite.CreatedByApp</span></span>    |

## <a name="http-request"></a><span data-ttu-id="06573-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="06573-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="06573-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="06573-117">Request headers</span></span>
|<span data-ttu-id="06573-118">Name</span><span class="sxs-lookup"><span data-stu-id="06573-118">Name</span></span> | <span data-ttu-id="06573-119">Typ</span><span class="sxs-lookup"><span data-stu-id="06573-119">Type</span></span> | <span data-ttu-id="06573-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06573-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="06573-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="06573-121">Authorization</span></span> | <span data-ttu-id="06573-122">string</span><span class="sxs-lookup"><span data-stu-id="06573-122">string</span></span> |<span data-ttu-id="06573-123">Der Authorization-Header wird verwendet, um die Anmeldeinformationen des Anrufers zu übergeben.</span><span class="sxs-lookup"><span data-stu-id="06573-123">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="06573-124">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="06573-124">Bearer {token}.</span></span> <span data-ttu-id="06573-125">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="06573-125">Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="06573-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="06573-126">Request body</span></span>
<span data-ttu-id="06573-127">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines Objekts [Benachrichtigung](../resources/projectrome-notification.md) .</span><span class="sxs-lookup"><span data-stu-id="06573-127">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="06573-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="06573-128">Response</span></span>
<span data-ttu-id="06573-129">Wenn der Vorgang erfolgreich war, gibt diese Methode die `201 Created` Antwortcode, der angibt, dass die Benachrichtigung erfolgreich erstellt und gespeichert wurde.</span><span class="sxs-lookup"><span data-stu-id="06573-129">If successful, this method returns the `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> 
## <a name="example"></a><span data-ttu-id="06573-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="06573-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="06573-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="06573-131">Request</span></span>
<span data-ttu-id="06573-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="06573-132">The following is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/me/notifications/
Content-type: application/json

{
    "targetHostName": "graphnotifications.sample.windows.com",
    "appNotificationId": "testDirectToastNotification",
    "expirationDateTime": "2018-08-29T23:51:33.000Z",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    },
    "targetPolicy": {
        "platformTypes": [
        "windows",
        "android"
        ]
    },
    "priority": "High",
    "groupName": "TestGroup",
    "displayTimeToLive": "23"
}
```

#### <a name="response"></a><span data-ttu-id="06573-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="06573-133">Response</span></span>
<span data-ttu-id="06573-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="06573-134">The following is an example of the response.</span></span>

```http
HTTP/1.1 201
Content-Type: application/json
location: https://graph.microsoft.com/beta/me/notifications/518c4fb1-c565-4d67-95c4-bcc3eb8eda1b

{
    "@odata.context": "https://graph.microsoft.com/test872018/$metadata#users('graphNotificationsUser%40contoso.com')/notifications/$entity",
    "appNotificationId": "testDirectToastNotification",
    "displayTimeToLive": 23,
    "expirationDateTime": "2018-08-24T12:31:53.858Z",
    "groupName": "TestGroup",
    "id": "cd5c5e6a-99ce-470a-9982-c47635e73620",
    "priority": "1",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    }
}
```


<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-notification-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
