---
title: eventMessage aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des eventMessage-Objekts.
ms.openlocfilehash: 3d81977c815737ae96839c6fc883692bf2555597
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058618"
---
# <a name="update-eventmessage"></a><span data-ttu-id="dd1c1-103">eventMessage aktualisieren</span><span class="sxs-lookup"><span data-stu-id="dd1c1-103">Update eventMessage</span></span>

> <span data-ttu-id="dd1c1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dd1c1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd1c1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dd1c1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dd1c1-106">Dient zum Aktualisieren der Eigenschaften des [eventMessage](../resources/eventmessage.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="dd1c1-106">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dd1c1-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dd1c1-107">Permissions</span></span>
<span data-ttu-id="dd1c1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd1c1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd1c1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dd1c1-110">Permission type</span></span>      | <span data-ttu-id="dd1c1-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dd1c1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd1c1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dd1c1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dd1c1-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd1c1-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dd1c1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dd1c1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd1c1-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd1c1-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dd1c1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dd1c1-116">Application</span></span> | <span data-ttu-id="dd1c1-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd1c1-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd1c1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd1c1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="dd1c1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dd1c1-119">Request headers</span></span>
| <span data-ttu-id="dd1c1-120">Name</span><span class="sxs-lookup"><span data-stu-id="dd1c1-120">Name</span></span>       | <span data-ttu-id="dd1c1-121">Typ</span><span class="sxs-lookup"><span data-stu-id="dd1c1-121">Type</span></span> | <span data-ttu-id="dd1c1-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd1c1-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dd1c1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd1c1-123">Authorization</span></span>  | <span data-ttu-id="dd1c1-124">string</span><span class="sxs-lookup"><span data-stu-id="dd1c1-124">string</span></span>  | <span data-ttu-id="dd1c1-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dd1c1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dd1c1-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd1c1-127">Content-Type</span></span> | <span data-ttu-id="dd1c1-128">string</span><span class="sxs-lookup"><span data-stu-id="dd1c1-128">string</span></span>  | <span data-ttu-id="dd1c1-p104">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dd1c1-p104">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="dd1c1-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dd1c1-131">Request body</span></span>
<span data-ttu-id="dd1c1-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben. Schreibbare/Aktualisierbare Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="dd1c1-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="dd1c1-136">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dd1c1-136">Property</span></span>     | <span data-ttu-id="dd1c1-137">Typ</span><span class="sxs-lookup"><span data-stu-id="dd1c1-137">Type</span></span>   |<span data-ttu-id="dd1c1-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd1c1-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd1c1-139">categories</span><span class="sxs-lookup"><span data-stu-id="dd1c1-139">categories</span></span>|<span data-ttu-id="dd1c1-140">String</span><span class="sxs-lookup"><span data-stu-id="dd1c1-140">String</span></span>|<span data-ttu-id="dd1c1-141">Die Kategorien, die mit der Nachricht verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="dd1c1-141">The categories associated with the message.</span></span>|
|<span data-ttu-id="dd1c1-142">importance</span><span class="sxs-lookup"><span data-stu-id="dd1c1-142">importance</span></span>|<span data-ttu-id="dd1c1-143">String</span><span class="sxs-lookup"><span data-stu-id="dd1c1-143">String</span></span>|<span data-ttu-id="dd1c1-p106">Wichtigkeit der Nachricht Mögliche Werte: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="dd1c1-p106">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="dd1c1-146">isAllDay</span><span class="sxs-lookup"><span data-stu-id="dd1c1-146">isAllDay</span></span> |<span data-ttu-id="dd1c1-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd1c1-147">Boolean</span></span>|<span data-ttu-id="dd1c1-148">Gibt an, ob das Ereignis den ganzen Tag dauert.</span><span class="sxs-lookup"><span data-stu-id="dd1c1-148">Indicates whether the event lasts the entire day.</span></span> <span data-ttu-id="dd1c1-149">Anpassen dieser Eigenschaft erfordert die **StartDateTime** und **EndDateTime** Eigenschaften des Ereignisses sowie anpassen.</span><span class="sxs-lookup"><span data-stu-id="dd1c1-149">Adjusting this property requires adjusting the **startDateTime** and **endDateTime** properties of the event as well.</span></span>|
|<span data-ttu-id="dd1c1-150">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="dd1c1-150">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="dd1c1-151">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dd1c1-151">Boolean</span></span>|<span data-ttu-id="dd1c1-152">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="dd1c1-152">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="dd1c1-153">isRead</span><span class="sxs-lookup"><span data-stu-id="dd1c1-153">isRead</span></span>|<span data-ttu-id="dd1c1-154">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dd1c1-154">Boolean</span></span>|<span data-ttu-id="dd1c1-155">Gibt an, ob die Nachricht gelesen wurde.</span><span class="sxs-lookup"><span data-stu-id="dd1c1-155">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="dd1c1-156">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="dd1c1-156">isReadReceiptRequested</span></span>|<span data-ttu-id="dd1c1-157">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dd1c1-157">Boolean</span></span>|<span data-ttu-id="dd1c1-158">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="dd1c1-158">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="dd1c1-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd1c1-159">Response</span></span>

<span data-ttu-id="dd1c1-160">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [eventMessage](../resources/eventmessage.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd1c1-160">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dd1c1-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dd1c1-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd1c1-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd1c1-162">Request</span></span>
<span data-ttu-id="dd1c1-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dd1c1-163">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="dd1c1-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd1c1-164">Response</span></span>
<span data-ttu-id="dd1c1-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd1c1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update eventmessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
