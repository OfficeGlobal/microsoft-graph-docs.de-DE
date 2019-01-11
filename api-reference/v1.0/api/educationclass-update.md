---
title: Educationclass-Eigenschaften aktualisieren
description: Dient zum Aktualisieren der Eigenschaften einer Klasse.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: ad91ddafc669e641cb21fb91bccfda4a1eea4dd1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894075"
---
# <a name="update-educationclass-properties"></a><span data-ttu-id="4390b-103">Educationclass-Eigenschaften aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4390b-103">Update educationclass properties</span></span>

<span data-ttu-id="4390b-104">Dient zum Aktualisieren der Eigenschaften einer Klasse.</span><span class="sxs-lookup"><span data-stu-id="4390b-104">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="4390b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4390b-105">Permissions</span></span>
<span data-ttu-id="4390b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4390b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4390b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4390b-108">Permission type</span></span>      | <span data-ttu-id="4390b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4390b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4390b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4390b-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="4390b-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4390b-111">Not supported.</span></span>  |
|<span data-ttu-id="4390b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4390b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4390b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4390b-113">Not supported.</span></span>   |
|<span data-ttu-id="4390b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4390b-114">Application</span></span> | <span data-ttu-id="4390b-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4390b-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4390b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4390b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4390b-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4390b-117">Request headers</span></span>
| <span data-ttu-id="4390b-118">Header</span><span class="sxs-lookup"><span data-stu-id="4390b-118">Header</span></span>       | <span data-ttu-id="4390b-119">Wert</span><span class="sxs-lookup"><span data-stu-id="4390b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4390b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4390b-120">Authorization</span></span>  | <span data-ttu-id="4390b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4390b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4390b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4390b-123">Content-Type</span></span>  | <span data-ttu-id="4390b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4390b-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4390b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4390b-125">Request body</span></span>
<span data-ttu-id="4390b-126">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="4390b-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4390b-127">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="4390b-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4390b-128">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="4390b-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4390b-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4390b-129">Property</span></span>     | <span data-ttu-id="4390b-130">Typ</span><span class="sxs-lookup"><span data-stu-id="4390b-130">Type</span></span>   |<span data-ttu-id="4390b-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4390b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4390b-132">description</span><span class="sxs-lookup"><span data-stu-id="4390b-132">description</span></span>|<span data-ttu-id="4390b-133">String</span><span class="sxs-lookup"><span data-stu-id="4390b-133">String</span></span>| <span data-ttu-id="4390b-134">Beschreibung der Klasse</span><span class="sxs-lookup"><span data-stu-id="4390b-134">Description of the class.</span></span>|
|<span data-ttu-id="4390b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4390b-135">displayName</span></span>|<span data-ttu-id="4390b-136">String</span><span class="sxs-lookup"><span data-stu-id="4390b-136">String</span></span>| <span data-ttu-id="4390b-137">Der Name der Klasse</span><span class="sxs-lookup"><span data-stu-id="4390b-137">Name of the class.</span></span>|
|<span data-ttu-id="4390b-138">mailNickname</span><span class="sxs-lookup"><span data-stu-id="4390b-138">mailNickname</span></span>|<span data-ttu-id="4390b-139">String</span><span class="sxs-lookup"><span data-stu-id="4390b-139">String</span></span>| <span data-ttu-id="4390b-140">E-Mail-Alias zum Senden von E-Mails an alle Benutzer, wenn diese Funktion aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="4390b-140">Email alias for sending email to all users if that feature is enabled.</span></span> |
<span data-ttu-id="4390b-141"><!-- Please verify the revised description here. -->| ClassCode | Zeichenfolge | Code für die Schule-Klasse. | | ExternalId | Zeichenfolge | Die ID der Klasse aus dem System synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="4390b-141"><!-- Please verify the revised description here. --> |classCode|String| Class code used by the school.| |externalId|String| ID of the class from the syncing system.</span></span> <span data-ttu-id="4390b-142">| |externalName|String| Name der Klasse im Synchronisierungssystem.| |externalSource|String| Wie diese Klasse erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="4390b-142">| |externalName|String|Name of the class in the syncing system.| |externalSource|string| How this class was created.</span></span> <span data-ttu-id="4390b-143">Die möglichen Werte sind: `sis`, `manual`, `enum_sentinel`. |</span><span class="sxs-lookup"><span data-stu-id="4390b-143">The possible values are: `sis`, `manual`, `enum_sentinel`.|</span></span>

## <a name="response"></a><span data-ttu-id="4390b-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="4390b-144">Response</span></span>
<span data-ttu-id="4390b-145">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [educationClass](../resources/educationclass.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4390b-145">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4390b-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4390b-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4390b-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4390b-147">Request</span></span>
<span data-ttu-id="4390b-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4390b-148">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationclass"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/classes/{class-id}
Content-type: application/json
Content-length: 224

{
  "description": "History - World History 1",
  "displayName": "World History Level 1",
}
```
##### <a name="response"></a><span data-ttu-id="4390b-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="4390b-149">Response</span></span>
<span data-ttu-id="4390b-150">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4390b-150">The following is an example of the response.</span></span> 

><span data-ttu-id="4390b-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="4390b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
