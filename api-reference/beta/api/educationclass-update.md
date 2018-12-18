---
title: Educationclass-Eigenschaften aktualisieren
description: Dient zum Aktualisieren der Eigenschaften einer Klasse.
author: mmast-msft
ms.openlocfilehash: 4215ebd25b8c4cf47663ad0a109b5d1aed784fda
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336666"
---
# <a name="update-educationclass-properties"></a><span data-ttu-id="3664b-103">Educationclass-Eigenschaften aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3664b-103">Update educationclass properties</span></span>

> <span data-ttu-id="3664b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3664b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3664b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3664b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3664b-106">Dient zum Aktualisieren der Eigenschaften einer Klasse.</span><span class="sxs-lookup"><span data-stu-id="3664b-106">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="3664b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3664b-107">Permissions</span></span>
<span data-ttu-id="3664b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3664b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3664b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3664b-110">Permission type</span></span>      | <span data-ttu-id="3664b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3664b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3664b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3664b-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="3664b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3664b-113">Not supported.</span></span>  |
|<span data-ttu-id="3664b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3664b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3664b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3664b-115">Not supported.</span></span>   |
|<span data-ttu-id="3664b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3664b-116">Application</span></span> | <span data-ttu-id="3664b-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3664b-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3664b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3664b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3664b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3664b-119">Request headers</span></span>
| <span data-ttu-id="3664b-120">Header</span><span class="sxs-lookup"><span data-stu-id="3664b-120">Header</span></span>       | <span data-ttu-id="3664b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3664b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3664b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3664b-122">Authorization</span></span>  | <span data-ttu-id="3664b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3664b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3664b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3664b-125">Content-Type</span></span>  | <span data-ttu-id="3664b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3664b-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3664b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3664b-127">Request body</span></span>
<span data-ttu-id="3664b-128">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="3664b-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3664b-129">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="3664b-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3664b-130">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="3664b-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3664b-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3664b-131">Property</span></span>     | <span data-ttu-id="3664b-132">Typ</span><span class="sxs-lookup"><span data-stu-id="3664b-132">Type</span></span>   |<span data-ttu-id="3664b-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3664b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3664b-134">description</span><span class="sxs-lookup"><span data-stu-id="3664b-134">description</span></span>|<span data-ttu-id="3664b-135">String</span><span class="sxs-lookup"><span data-stu-id="3664b-135">String</span></span>| <span data-ttu-id="3664b-136">Beschreibung der Klasse</span><span class="sxs-lookup"><span data-stu-id="3664b-136">Description of the class.</span></span>|
|<span data-ttu-id="3664b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3664b-137">displayName</span></span>|<span data-ttu-id="3664b-138">String</span><span class="sxs-lookup"><span data-stu-id="3664b-138">String</span></span>| <span data-ttu-id="3664b-139">Der Name der Klasse</span><span class="sxs-lookup"><span data-stu-id="3664b-139">Name of the class.</span></span>|
|<span data-ttu-id="3664b-140">mailNickname</span><span class="sxs-lookup"><span data-stu-id="3664b-140">mailNickname</span></span>|<span data-ttu-id="3664b-141">String</span><span class="sxs-lookup"><span data-stu-id="3664b-141">String</span></span>| <span data-ttu-id="3664b-142">E-Mail-Alias zum Senden von E-Mails an alle Benutzer, wenn diese Funktion aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="3664b-142">Email alias for sending email to all users if that feature is enabled.</span></span> |
<span data-ttu-id="3664b-143"><!-- Please verify the revised description here. -->| ClassCode | Zeichenfolge | Code für die Schule-Klasse. | | ExternalId | Zeichenfolge | Die ID der Klasse aus dem System synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="3664b-143"><!-- Please verify the revised description here. --> |classCode|String| Class code used by the school.| |externalId|String| ID of the class from the syncing system.</span></span> <span data-ttu-id="3664b-144">| |externalName|String| Name der Klasse im Synchronisierungssystem.| |externalSource|String| Wie diese Klasse erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="3664b-144">| |externalName|String|Name of the class in the syncing system.| |externalSource|string| How this class was created.</span></span> <span data-ttu-id="3664b-145">Mögliche Werte: `sis`, `manual`, `enum_sentinel`.|</span><span class="sxs-lookup"><span data-stu-id="3664b-145">Possible values are: `sis`, `manual`, `enum_sentinel`.|</span></span>

## <a name="response"></a><span data-ttu-id="3664b-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="3664b-146">Response</span></span>
<span data-ttu-id="3664b-147">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [educationClass](../resources/educationclass.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3664b-147">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3664b-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3664b-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3664b-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3664b-149">Request</span></span>
<span data-ttu-id="3664b-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3664b-150">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationclass"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11014
Content-type: application/json
Content-length: 224

{
  "description": "History - World History 1",
  "displayName": "World History Level 1",
}
```
##### <a name="response"></a><span data-ttu-id="3664b-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="3664b-151">Response</span></span>
<span data-ttu-id="3664b-152">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3664b-152">The following is an example of the response.</span></span> 

><span data-ttu-id="3664b-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="3664b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11014",
  "description": "World History Level 1",
  "classCode": "301",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
  "displayName": "History - World History 1",
  "externalId": "301",
  "externalName": "World History Level 1",
  "externalSource": "Fabrikam High School",
  "mailNickname": "Fabrikam"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationclass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->