---
title: Erstellen Sie und senden Sie eine Benachrichtigung
description: 'Erstellen Sie und senden Sie eine Benachrichtigung für einen Benutzer über Microsoft Graph. Die Benachrichtigung wird in der Microsoft Graph-Benachrichtigung feed Store gespeichert und an alle Geräte-Endpunkten, bei denen der Benutzer, in angemeldet ist allen app-Clients gesendet.  '
localization_priority: Normal
ms.openlocfilehash: 67906aa56ace21d9d03cfe47c17acda38d8c680f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843898"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="6d4d5-104">Erstellen Sie und senden Sie eine Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="6d4d5-104">Create and send a notification</span></span>
> <span data-ttu-id="6d4d5-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6d4d5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d4d5-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6d4d5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6d4d5-107">Erstellen Sie und senden Sie eine Benachrichtigung für einen Benutzer über Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6d4d5-107">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="6d4d5-108">Die Benachrichtigung wird in der Microsoft Graph-Benachrichtigung feed Store gespeichert und an alle Geräte-Endpunkten, bei denen der Benutzer, in angemeldet ist allen app-Clients gesendet.</span><span class="sxs-lookup"><span data-stu-id="6d4d5-108">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  
## <a name="permissions"></a><span data-ttu-id="6d4d5-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6d4d5-109">Permissions</span></span>
<span data-ttu-id="6d4d5-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d4d5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d4d5-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6d4d5-112">Permission type</span></span>      | <span data-ttu-id="6d4d5-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6d4d5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d4d5-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6d4d5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6d4d5-115">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="6d4d5-115">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="6d4d5-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6d4d5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d4d5-117">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="6d4d5-117">Notifications.ReadWrite.CreatedByApp</span></span>    |

## <a name="http-request"></a><span data-ttu-id="6d4d5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d4d5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="6d4d5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6d4d5-119">Request headers</span></span>
|<span data-ttu-id="6d4d5-120">Name</span><span class="sxs-lookup"><span data-stu-id="6d4d5-120">Name</span></span> | <span data-ttu-id="6d4d5-121">Typ</span><span class="sxs-lookup"><span data-stu-id="6d4d5-121">Type</span></span> | <span data-ttu-id="6d4d5-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d4d5-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="6d4d5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d4d5-123">Authorization</span></span> | <span data-ttu-id="6d4d5-124">string</span><span class="sxs-lookup"><span data-stu-id="6d4d5-124">string</span></span> |<span data-ttu-id="6d4d5-125">Der Authorization-Header wird verwendet, um die Anmeldeinformationen des Anrufers zu übergeben.</span><span class="sxs-lookup"><span data-stu-id="6d4d5-125">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="6d4d5-126">Bearer {Token}.</span><span class="sxs-lookup"><span data-stu-id="6d4d5-126">Bearer {token}.</span></span> <span data-ttu-id="6d4d5-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6d4d5-127">Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="6d4d5-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6d4d5-128">Request body</span></span>
<span data-ttu-id="6d4d5-129">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines Objekts [Benachrichtigung](../resources/projectrome-notification.md) .</span><span class="sxs-lookup"><span data-stu-id="6d4d5-129">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6d4d5-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d4d5-130">Response</span></span>
<span data-ttu-id="6d4d5-131">Wenn der Vorgang erfolgreich war, gibt diese Methode die `201 Created` Antwortcode, der angibt, dass die Benachrichtigung erfolgreich erstellt und gespeichert wurde.</span><span class="sxs-lookup"><span data-stu-id="6d4d5-131">If successful, this method returns the `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> 
## <a name="example"></a><span data-ttu-id="6d4d5-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6d4d5-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6d4d5-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d4d5-133">Request</span></span>
<span data-ttu-id="6d4d5-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6d4d5-134">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="6d4d5-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d4d5-135">Response</span></span>
<span data-ttu-id="6d4d5-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6d4d5-136">The following is an example of the response.</span></span>

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


