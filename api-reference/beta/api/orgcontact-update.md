---
title: Orgcontact aktualisieren
description: Aktualisieren Sie die Eigenschaften des Orgcontact-Objekts.
localization_priority: Normal
ms.openlocfilehash: f48795bef6ea1a4833379f54747cbf2c291b2454
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859066"
---
# <a name="update-orgcontact"></a><span data-ttu-id="ec541-103">Orgcontact aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ec541-103">Update orgcontact</span></span>

> <span data-ttu-id="ec541-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ec541-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec541-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ec541-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ec541-106">Aktualisieren Sie die Eigenschaften des Orgcontact-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ec541-106">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ec541-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ec541-107">Permissions</span></span>
<span data-ttu-id="ec541-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec541-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec541-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ec541-110">Permission type</span></span>      | <span data-ttu-id="ec541-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ec541-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec541-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ec541-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ec541-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec541-113">Not supported.</span></span>    |
|<span data-ttu-id="ec541-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ec541-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec541-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec541-115">Not supported.</span></span>    |
|<span data-ttu-id="ec541-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ec541-116">Application</span></span> | <span data-ttu-id="ec541-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec541-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec541-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec541-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ec541-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ec541-119">Request headers</span></span>
| <span data-ttu-id="ec541-120">Name</span><span class="sxs-lookup"><span data-stu-id="ec541-120">Name</span></span>       | <span data-ttu-id="ec541-121">Typ</span><span class="sxs-lookup"><span data-stu-id="ec541-121">Type</span></span> | <span data-ttu-id="ec541-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec541-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ec541-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec541-123">Authorization</span></span>  | <span data-ttu-id="ec541-124">string</span><span class="sxs-lookup"><span data-stu-id="ec541-124">string</span></span>  | <span data-ttu-id="ec541-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ec541-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec541-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ec541-127">Request body</span></span>
<span data-ttu-id="ec541-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="ec541-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ec541-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ec541-131">Property</span></span>     | <span data-ttu-id="ec541-132">Typ</span><span class="sxs-lookup"><span data-stu-id="ec541-132">Type</span></span>   |<span data-ttu-id="ec541-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec541-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec541-134">city</span><span class="sxs-lookup"><span data-stu-id="ec541-134">city</span></span>|<span data-ttu-id="ec541-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ec541-135">String</span></span>||
|<span data-ttu-id="ec541-136">Land</span><span class="sxs-lookup"><span data-stu-id="ec541-136">country</span></span>|<span data-ttu-id="ec541-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ec541-137">String</span></span>||
|<span data-ttu-id="ec541-138">department</span><span class="sxs-lookup"><span data-stu-id="ec541-138">department</span></span>|<span data-ttu-id="ec541-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ec541-139">String</span></span>||
|<span data-ttu-id="ec541-140">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="ec541-140">onPremisesSyncEnabled</span></span>|<span data-ttu-id="ec541-141">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ec541-141">Boolean</span></span>||
|<span data-ttu-id="ec541-142">displayName</span><span class="sxs-lookup"><span data-stu-id="ec541-142">displayName</span></span>|<span data-ttu-id="ec541-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ec541-143">String</span></span>||
|<span data-ttu-id="ec541-144">givenName</span><span class="sxs-lookup"><span data-stu-id="ec541-144">givenName</span></span>|<span data-ttu-id="ec541-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ec541-145">String</span></span>||
|<span data-ttu-id="ec541-146">jobTitle</span><span class="sxs-lookup"><span data-stu-id="ec541-146">jobTitle</span></span>|<span data-ttu-id="ec541-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ec541-147">String</span></span>||
|<span data-ttu-id="ec541-148">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ec541-148">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="ec541-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec541-149">DateTimeOffset</span></span>||
|<span data-ttu-id="ec541-150">mail</span><span class="sxs-lookup"><span data-stu-id="ec541-150">mail</span></span>|<span data-ttu-id="ec541-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ec541-151">String</span></span>||
|<span data-ttu-id="ec541-152">mailNickname</span><span class="sxs-lookup"><span data-stu-id="ec541-152">mailNickname</span></span>|<span data-ttu-id="ec541-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ec541-153">String</span></span>||
|<span data-ttu-id="ec541-154">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="ec541-154">mobilePhone</span></span>|<span data-ttu-id="ec541-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ec541-155">String</span></span>||
|<span data-ttu-id="ec541-156">officeLocation</span><span class="sxs-lookup"><span data-stu-id="ec541-156">officeLocation</span></span>|<span data-ttu-id="ec541-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ec541-157">String</span></span>||
|<span data-ttu-id="ec541-158">postalCode</span><span class="sxs-lookup"><span data-stu-id="ec541-158">postalCode</span></span>|<span data-ttu-id="ec541-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ec541-159">String</span></span>||
|<span data-ttu-id="ec541-160">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="ec541-160">proxyAddresses</span></span>|<span data-ttu-id="ec541-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ec541-161">String</span></span>||
|<span data-ttu-id="ec541-162">state</span><span class="sxs-lookup"><span data-stu-id="ec541-162">state</span></span>|<span data-ttu-id="ec541-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ec541-163">String</span></span>||
|<span data-ttu-id="ec541-164">streetAddress</span><span class="sxs-lookup"><span data-stu-id="ec541-164">streetAddress</span></span>|<span data-ttu-id="ec541-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ec541-165">String</span></span>||
|<span data-ttu-id="ec541-166">surname</span><span class="sxs-lookup"><span data-stu-id="ec541-166">surname</span></span>|<span data-ttu-id="ec541-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ec541-167">String</span></span>||
|<span data-ttu-id="ec541-168">businessPhones</span><span class="sxs-lookup"><span data-stu-id="ec541-168">businessPhones</span></span>|<span data-ttu-id="ec541-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ec541-169">String</span></span>||

## <a name="response"></a><span data-ttu-id="ec541-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec541-170">Response</span></span>

<span data-ttu-id="ec541-171">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [OrgContact](../resources/orgcontact.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ec541-171">If successful, this method returns a `200 OK` response code and updated [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ec541-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ec541-172">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec541-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec541-173">Request</span></span>
<span data-ttu-id="ec541-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ec541-174">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="ec541-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec541-175">Response</span></span>
<span data-ttu-id="ec541-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ec541-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update orgcontact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
