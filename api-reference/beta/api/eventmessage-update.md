---
title: eventMessage aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des eventMessage-Objekts.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 160fbf70f243174265fc6e4e54feabb8042bd450
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513585"
---
# <a name="update-eventmessage"></a><span data-ttu-id="136b0-103">eventMessage aktualisieren</span><span class="sxs-lookup"><span data-stu-id="136b0-103">Update eventMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="136b0-104">Dient zum Aktualisieren der Eigenschaften des [eventMessage](../resources/eventmessage.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="136b0-104">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="136b0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="136b0-105">Permissions</span></span>
<span data-ttu-id="136b0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="136b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="136b0-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="136b0-108">Permission type</span></span>      | <span data-ttu-id="136b0-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="136b0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="136b0-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="136b0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="136b0-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="136b0-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="136b0-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="136b0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="136b0-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="136b0-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="136b0-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="136b0-114">Application</span></span> | <span data-ttu-id="136b0-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="136b0-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="136b0-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="136b0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="136b0-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="136b0-117">Request headers</span></span>
| <span data-ttu-id="136b0-118">Name</span><span class="sxs-lookup"><span data-stu-id="136b0-118">Name</span></span>       | <span data-ttu-id="136b0-119">Typ</span><span class="sxs-lookup"><span data-stu-id="136b0-119">Type</span></span> | <span data-ttu-id="136b0-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="136b0-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="136b0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="136b0-121">Authorization</span></span>  | <span data-ttu-id="136b0-122">string</span><span class="sxs-lookup"><span data-stu-id="136b0-122">string</span></span>  | <span data-ttu-id="136b0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="136b0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="136b0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="136b0-125">Content-Type</span></span> | <span data-ttu-id="136b0-126">string</span><span class="sxs-lookup"><span data-stu-id="136b0-126">string</span></span>  | <span data-ttu-id="136b0-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="136b0-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="136b0-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="136b0-129">Request body</span></span>
<span data-ttu-id="136b0-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben. Schreibbare/Aktualisierbare Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="136b0-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="136b0-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="136b0-134">Property</span></span>     | <span data-ttu-id="136b0-135">Typ</span><span class="sxs-lookup"><span data-stu-id="136b0-135">Type</span></span>   |<span data-ttu-id="136b0-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="136b0-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="136b0-137">categories</span><span class="sxs-lookup"><span data-stu-id="136b0-137">categories</span></span>|<span data-ttu-id="136b0-138">String</span><span class="sxs-lookup"><span data-stu-id="136b0-138">String</span></span>|<span data-ttu-id="136b0-139">Die Kategorien, die mit der Nachricht verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="136b0-139">The categories associated with the message.</span></span>|
|<span data-ttu-id="136b0-140">importance</span><span class="sxs-lookup"><span data-stu-id="136b0-140">importance</span></span>|<span data-ttu-id="136b0-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="136b0-141">String</span></span>|<span data-ttu-id="136b0-p105">Wichtigkeit der Nachricht Mögliche Werte: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="136b0-p105">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="136b0-144">isAllDay</span><span class="sxs-lookup"><span data-stu-id="136b0-144">isAllDay</span></span> |<span data-ttu-id="136b0-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="136b0-145">Boolean</span></span>|<span data-ttu-id="136b0-146">Gibt an, ob das Ereignis den ganzen Tag dauert.</span><span class="sxs-lookup"><span data-stu-id="136b0-146">Indicates whether the event lasts the entire day.</span></span> <span data-ttu-id="136b0-147">Anpassen dieser Eigenschaft erfordert die **StartDateTime** und **EndDateTime** Eigenschaften des Ereignisses sowie anpassen.</span><span class="sxs-lookup"><span data-stu-id="136b0-147">Adjusting this property requires adjusting the **startDateTime** and **endDateTime** properties of the event as well.</span></span>|
|<span data-ttu-id="136b0-148">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="136b0-148">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="136b0-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="136b0-149">Boolean</span></span>|<span data-ttu-id="136b0-150">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="136b0-150">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="136b0-151">isRead</span><span class="sxs-lookup"><span data-stu-id="136b0-151">isRead</span></span>|<span data-ttu-id="136b0-152">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="136b0-152">Boolean</span></span>|<span data-ttu-id="136b0-153">Gibt an, ob die Nachricht gelesen wurde.</span><span class="sxs-lookup"><span data-stu-id="136b0-153">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="136b0-154">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="136b0-154">isReadReceiptRequested</span></span>|<span data-ttu-id="136b0-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="136b0-155">Boolean</span></span>|<span data-ttu-id="136b0-156">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="136b0-156">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="136b0-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="136b0-157">Response</span></span>

<span data-ttu-id="136b0-158">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [eventMessage](../resources/eventmessage.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="136b0-158">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="136b0-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="136b0-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="136b0-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="136b0-160">Request</span></span>
<span data-ttu-id="136b0-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="136b0-161">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_eventmessage"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "isRead": "true",
}
```
##### <a name="response"></a><span data-ttu-id="136b0-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="136b0-162">Response</span></span>
<span data-ttu-id="136b0-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="136b0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "meetingMessageType": "meetingMessageType-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update eventmessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/eventmessage-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
