---
title: ConnectorGroups aktualisieren
description: Aktualisieren Sie die Eigenschaften des Connectorgroup-Objekts.
localization_priority: Normal
ms.openlocfilehash: 9a4db622328edd4d3aea348fd078acdc832a9c52
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843799"
---
# <a name="update-connectorgroups"></a><span data-ttu-id="d478b-103">ConnectorGroups aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d478b-103">Update connectorGroups</span></span>

> <span data-ttu-id="d478b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d478b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d478b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d478b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d478b-106">Aktualisieren Sie die Eigenschaften des Connectorgroup-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d478b-106">Update the properties of connectorgroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d478b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d478b-107">Permissions</span></span>
<span data-ttu-id="d478b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d478b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d478b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d478b-110">Permission type</span></span>      | <span data-ttu-id="d478b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d478b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d478b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d478b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d478b-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d478b-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d478b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d478b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d478b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d478b-115">Not supported.</span></span>    |
|<span data-ttu-id="d478b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d478b-116">Application</span></span> | <span data-ttu-id="d478b-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d478b-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d478b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d478b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /connectorGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="d478b-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d478b-119">Optional request headers</span></span>
| <span data-ttu-id="d478b-120">Name</span><span class="sxs-lookup"><span data-stu-id="d478b-120">Name</span></span>       | <span data-ttu-id="d478b-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d478b-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d478b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d478b-122">Authorization</span></span>  | <span data-ttu-id="d478b-123">Bearer.</span><span class="sxs-lookup"><span data-stu-id="d478b-123">Bearer.</span></span> <span data-ttu-id="d478b-124">Erforderlich</span><span class="sxs-lookup"><span data-stu-id="d478b-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="d478b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d478b-125">Request body</span></span>
<span data-ttu-id="d478b-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="d478b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d478b-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d478b-129">Property</span></span>     | <span data-ttu-id="d478b-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d478b-130">Type</span></span>   |<span data-ttu-id="d478b-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d478b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d478b-132">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="d478b-132">connectorGroupType</span></span>|<span data-ttu-id="d478b-133">string</span><span class="sxs-lookup"><span data-stu-id="d478b-133">string</span></span>| <span data-ttu-id="d478b-134">Mögliche Werte sind: `applicationProxy`.</span><span class="sxs-lookup"><span data-stu-id="d478b-134">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="d478b-135">name</span><span class="sxs-lookup"><span data-stu-id="d478b-135">name</span></span>|<span data-ttu-id="d478b-136">String</span><span class="sxs-lookup"><span data-stu-id="d478b-136">String</span></span>|<span data-ttu-id="d478b-137">Der Name der ConnectorGroup.</span><span class="sxs-lookup"><span data-stu-id="d478b-137">The name of the connectorGroup.</span></span>|

## <a name="response"></a><span data-ttu-id="d478b-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="d478b-138">Response</span></span>

<span data-ttu-id="d478b-139">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [ConnectorGroup](../resources/connectorgroup.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d478b-139">If successful, this method returns a `200 OK` response code and updated [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d478b-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d478b-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d478b-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d478b-141">Request</span></span>
<span data-ttu-id="d478b-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d478b-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup"
}-->
```http
PATCH https://graph.microsoft.com/{ver}/connectorGroups/{id}
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
}
```
##### <a name="response"></a><span data-ttu-id="d478b-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="d478b-143">Response</span></span>
<span data-ttu-id="d478b-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d478b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update connectorgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
