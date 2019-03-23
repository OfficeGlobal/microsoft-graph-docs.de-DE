---
title: Organisationskontakt aktualisieren
description: Aktualisieren der Eigenschaften des Organisationskontakt-Objekts.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cec4817472fe5192c7af836131cea83bcb60d77b
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/23/2019
ms.locfileid: "30789634"
---
# <a name="update-orgcontact"></a><span data-ttu-id="da6b0-103">Organisationskontakt aktualisieren</span><span class="sxs-lookup"><span data-stu-id="da6b0-103">Update orgcontact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da6b0-104">Aktualisieren der Eigenschaften des Organisationskontakt-Objekts.</span><span class="sxs-lookup"><span data-stu-id="da6b0-104">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="da6b0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="da6b0-105">Permissions</span></span>
<span data-ttu-id="da6b0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da6b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da6b0-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="da6b0-108">Permission type</span></span>      | <span data-ttu-id="da6b0-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="da6b0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da6b0-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="da6b0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="da6b0-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da6b0-111">Not supported.</span></span>    |
|<span data-ttu-id="da6b0-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="da6b0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da6b0-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da6b0-113">Not supported.</span></span>    |
|<span data-ttu-id="da6b0-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="da6b0-114">Application</span></span> | <span data-ttu-id="da6b0-115">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="da6b0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="da6b0-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="da6b0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="da6b0-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="da6b0-117">Request headers</span></span>
| <span data-ttu-id="da6b0-118">Name</span><span class="sxs-lookup"><span data-stu-id="da6b0-118">Name</span></span>       | <span data-ttu-id="da6b0-119">Typ</span><span class="sxs-lookup"><span data-stu-id="da6b0-119">Type</span></span> | <span data-ttu-id="da6b0-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da6b0-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="da6b0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="da6b0-121">Authorization</span></span>  | <span data-ttu-id="da6b0-122">string</span><span class="sxs-lookup"><span data-stu-id="da6b0-122">string</span></span>  | <span data-ttu-id="da6b0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="da6b0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da6b0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="da6b0-125">Request body</span></span>
<span data-ttu-id="da6b0-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="da6b0-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="da6b0-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="da6b0-129">Property</span></span>     | <span data-ttu-id="da6b0-130">Typ</span><span class="sxs-lookup"><span data-stu-id="da6b0-130">Type</span></span>   |<span data-ttu-id="da6b0-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da6b0-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da6b0-132">city</span><span class="sxs-lookup"><span data-stu-id="da6b0-132">city</span></span>|<span data-ttu-id="da6b0-133">String</span><span class="sxs-lookup"><span data-stu-id="da6b0-133">String</span></span>||
|<span data-ttu-id="da6b0-134">Land</span><span class="sxs-lookup"><span data-stu-id="da6b0-134">country</span></span>|<span data-ttu-id="da6b0-135">String</span><span class="sxs-lookup"><span data-stu-id="da6b0-135">String</span></span>||
|<span data-ttu-id="da6b0-136">department</span><span class="sxs-lookup"><span data-stu-id="da6b0-136">department</span></span>|<span data-ttu-id="da6b0-137">String</span><span class="sxs-lookup"><span data-stu-id="da6b0-137">String</span></span>||
|<span data-ttu-id="da6b0-138">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="da6b0-138">onPremisesSyncEnabled</span></span>|<span data-ttu-id="da6b0-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="da6b0-139">Boolean</span></span>||
|<span data-ttu-id="da6b0-140">displayName</span><span class="sxs-lookup"><span data-stu-id="da6b0-140">displayName</span></span>|<span data-ttu-id="da6b0-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da6b0-141">String</span></span>||
|<span data-ttu-id="da6b0-142">givenName</span><span class="sxs-lookup"><span data-stu-id="da6b0-142">givenName</span></span>|<span data-ttu-id="da6b0-143">String</span><span class="sxs-lookup"><span data-stu-id="da6b0-143">String</span></span>||
|<span data-ttu-id="da6b0-144">jobTitle</span><span class="sxs-lookup"><span data-stu-id="da6b0-144">jobTitle</span></span>|<span data-ttu-id="da6b0-145">String</span><span class="sxs-lookup"><span data-stu-id="da6b0-145">String</span></span>||
|<span data-ttu-id="da6b0-146">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="da6b0-146">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="da6b0-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da6b0-147">DateTimeOffset</span></span>||
|<span data-ttu-id="da6b0-148">mail</span><span class="sxs-lookup"><span data-stu-id="da6b0-148">mail</span></span>|<span data-ttu-id="da6b0-149">String</span><span class="sxs-lookup"><span data-stu-id="da6b0-149">String</span></span>||
|<span data-ttu-id="da6b0-150">mailNickname</span><span class="sxs-lookup"><span data-stu-id="da6b0-150">mailNickname</span></span>|<span data-ttu-id="da6b0-151">String</span><span class="sxs-lookup"><span data-stu-id="da6b0-151">String</span></span>||
|<span data-ttu-id="da6b0-152">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="da6b0-152">mobilePhone</span></span>|<span data-ttu-id="da6b0-153">String</span><span class="sxs-lookup"><span data-stu-id="da6b0-153">String</span></span>||
|<span data-ttu-id="da6b0-154">officeLocation</span><span class="sxs-lookup"><span data-stu-id="da6b0-154">officeLocation</span></span>|<span data-ttu-id="da6b0-155">String</span><span class="sxs-lookup"><span data-stu-id="da6b0-155">String</span></span>||
|<span data-ttu-id="da6b0-156">postalCode</span><span class="sxs-lookup"><span data-stu-id="da6b0-156">postalCode</span></span>|<span data-ttu-id="da6b0-157">String</span><span class="sxs-lookup"><span data-stu-id="da6b0-157">String</span></span>||
|<span data-ttu-id="da6b0-158">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="da6b0-158">proxyAddresses</span></span>|<span data-ttu-id="da6b0-159">String</span><span class="sxs-lookup"><span data-stu-id="da6b0-159">String</span></span>||
|<span data-ttu-id="da6b0-160">state</span><span class="sxs-lookup"><span data-stu-id="da6b0-160">state</span></span>|<span data-ttu-id="da6b0-161">String</span><span class="sxs-lookup"><span data-stu-id="da6b0-161">String</span></span>||
|<span data-ttu-id="da6b0-162">streetAddress</span><span class="sxs-lookup"><span data-stu-id="da6b0-162">streetAddress</span></span>|<span data-ttu-id="da6b0-163">String</span><span class="sxs-lookup"><span data-stu-id="da6b0-163">String</span></span>||
|<span data-ttu-id="da6b0-164">surname</span><span class="sxs-lookup"><span data-stu-id="da6b0-164">surname</span></span>|<span data-ttu-id="da6b0-165">String</span><span class="sxs-lookup"><span data-stu-id="da6b0-165">String</span></span>||
|<span data-ttu-id="da6b0-166">businessPhones</span><span class="sxs-lookup"><span data-stu-id="da6b0-166">businessPhones</span></span>|<span data-ttu-id="da6b0-167">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="da6b0-167">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="da6b0-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="da6b0-168">Response</span></span>

<span data-ttu-id="da6b0-169">Bei erfolgreicher Ausführung gibt diese Methode einen `200 OK` Antwortcode und ein aktualisiertes [Organisationskontakt](../resources/orgcontact.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="da6b0-169">If successful, this method returns a `200 OK` response code and updated [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="da6b0-170">Beispiel</span><span class="sxs-lookup"><span data-stu-id="da6b0-170">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da6b0-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="da6b0-171">Request</span></span>
<span data-ttu-id="da6b0-172">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="da6b0-172">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_orgcontact"
}-->
```http
PATCH https://graph.microsoft.com/beta/contacts/{id}
Content-type: application/json
Content-length: 222

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value",
  "country": "country-value",
  "department": "department-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="da6b0-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="da6b0-173">Response</span></span>
<span data-ttu-id="da6b0-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="da6b0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value",
  "country": "country-value",
  "department": "department-value",
  "displayName": "displayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update orgcontact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
