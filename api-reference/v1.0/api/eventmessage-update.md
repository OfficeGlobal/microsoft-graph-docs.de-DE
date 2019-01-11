---
title: eventMessage aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des eventMessage-Objekts.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 128849b2b0a1a156ef68498b345ca30833922d82
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867697"
---
# <a name="update-eventmessage"></a><span data-ttu-id="706ee-103">eventMessage aktualisieren</span><span class="sxs-lookup"><span data-stu-id="706ee-103">Update eventMessage</span></span>

<span data-ttu-id="706ee-104">Dient zum Aktualisieren der Eigenschaften des [eventMessage](../resources/eventmessage.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="706ee-104">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="706ee-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="706ee-105">Permissions</span></span>
<span data-ttu-id="706ee-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="706ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="706ee-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="706ee-108">Permission type</span></span>      | <span data-ttu-id="706ee-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="706ee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="706ee-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="706ee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="706ee-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="706ee-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="706ee-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="706ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="706ee-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="706ee-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="706ee-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="706ee-114">Application</span></span> | <span data-ttu-id="706ee-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="706ee-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="706ee-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="706ee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="706ee-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="706ee-117">Request headers</span></span>
| <span data-ttu-id="706ee-118">Name</span><span class="sxs-lookup"><span data-stu-id="706ee-118">Name</span></span>       | <span data-ttu-id="706ee-119">Typ</span><span class="sxs-lookup"><span data-stu-id="706ee-119">Type</span></span> | <span data-ttu-id="706ee-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="706ee-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="706ee-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="706ee-121">Authorization</span></span>  | <span data-ttu-id="706ee-122">string</span><span class="sxs-lookup"><span data-stu-id="706ee-122">string</span></span>  | <span data-ttu-id="706ee-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="706ee-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="706ee-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="706ee-125">Content-Type</span></span> | <span data-ttu-id="706ee-126">string</span><span class="sxs-lookup"><span data-stu-id="706ee-126">string</span></span>  | <span data-ttu-id="706ee-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="706ee-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="706ee-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="706ee-129">Request body</span></span>
<span data-ttu-id="706ee-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben. Schreibbare/Aktualisierbare Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="706ee-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="706ee-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="706ee-134">Property</span></span>     | <span data-ttu-id="706ee-135">Typ</span><span class="sxs-lookup"><span data-stu-id="706ee-135">Type</span></span>   |<span data-ttu-id="706ee-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="706ee-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="706ee-137">categories</span><span class="sxs-lookup"><span data-stu-id="706ee-137">categories</span></span>|<span data-ttu-id="706ee-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="706ee-138">String</span></span>|<span data-ttu-id="706ee-139">Die Kategorien, die mit der Nachricht verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="706ee-139">The categories associated with the message.</span></span>|
|<span data-ttu-id="706ee-140">importance</span><span class="sxs-lookup"><span data-stu-id="706ee-140">importance</span></span>|<span data-ttu-id="706ee-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="706ee-141">String</span></span>|<span data-ttu-id="706ee-142">Die Wichtigkeit der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="706ee-142">The importance of the message.</span></span> <span data-ttu-id="706ee-143">Die möglichen Werte sind: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="706ee-143">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="706ee-144">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="706ee-144">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="706ee-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="706ee-145">Boolean</span></span>|<span data-ttu-id="706ee-146">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="706ee-146">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="706ee-147">isRead</span><span class="sxs-lookup"><span data-stu-id="706ee-147">isRead</span></span>|<span data-ttu-id="706ee-148">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="706ee-148">Boolean</span></span>|<span data-ttu-id="706ee-149">Gibt an, ob die Nachricht gelesen wurde.</span><span class="sxs-lookup"><span data-stu-id="706ee-149">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="706ee-150">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="706ee-150">isReadReceiptRequested</span></span>|<span data-ttu-id="706ee-151">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="706ee-151">Boolean</span></span>|<span data-ttu-id="706ee-152">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="706ee-152">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="706ee-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="706ee-153">Response</span></span>

<span data-ttu-id="706ee-154">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [eventMessage](../resources/eventmessage.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="706ee-154">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="706ee-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="706ee-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="706ee-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="706ee-156">Request</span></span>
<span data-ttu-id="706ee-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="706ee-157">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_eventmessage"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "isRead": "true",
}
```
##### <a name="response"></a><span data-ttu-id="706ee-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="706ee-158">Response</span></span>
<span data-ttu-id="706ee-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="706ee-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
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
