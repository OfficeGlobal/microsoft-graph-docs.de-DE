---
title: 'Benutzer: TranslateExchangeIds'
description: Übersetzen Sie IDs von Outlook-bezogene Ressourcen zwischen den Formaten.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3b09ae9bf6a1cbf1967a900770b07d8c9750ba21
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571289"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="b0563-103">Benutzer: TranslateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="b0563-103">user: translateExchangeIds</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0563-104">Übersetzen Sie IDs von Outlook-bezogene Ressourcen zwischen den Formaten.</span><span class="sxs-lookup"><span data-stu-id="b0563-104">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0563-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b0563-105">Permissions</span></span>

<span data-ttu-id="b0563-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0563-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b0563-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b0563-108">Permission type</span></span> | <span data-ttu-id="b0563-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b0563-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="b0563-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b0563-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b0563-111">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0563-111">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b0563-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b0563-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0563-113">User.ReadBasic, User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0563-113">User.ReadBasic, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="b0563-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b0563-114">Application</span></span> | <span data-ttu-id="b0563-115">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0563-115">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0563-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0563-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="b0563-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b0563-117">Request headers</span></span>

| <span data-ttu-id="b0563-118">Name</span><span class="sxs-lookup"><span data-stu-id="b0563-118">Name</span></span> | <span data-ttu-id="b0563-119">Wert</span><span class="sxs-lookup"><span data-stu-id="b0563-119">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="b0563-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0563-120">Authorization</span></span> | <span data-ttu-id="b0563-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b0563-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0563-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b0563-123">Request body</span></span>

| <span data-ttu-id="b0563-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="b0563-124">Parameter</span></span> | <span data-ttu-id="b0563-125">Typ</span><span class="sxs-lookup"><span data-stu-id="b0563-125">Type</span></span> | <span data-ttu-id="b0563-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0563-126">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="b0563-127">inputIds</span><span class="sxs-lookup"><span data-stu-id="b0563-127">inputIds</span></span> | <span data-ttu-id="b0563-128">Edm.String-Auflistung</span><span class="sxs-lookup"><span data-stu-id="b0563-128">Edm.String collection</span></span> | <span data-ttu-id="b0563-129">Eine Sammlung von Bezeichnern zu konvertieren.</span><span class="sxs-lookup"><span data-stu-id="b0563-129">A collection of identifiers to convert.</span></span> <span data-ttu-id="b0563-130">Alle Bezeichner in der Auflistung der gleichen ID Quelltyp benötigen und für Elemente im selben Postfach werden müssen.</span><span class="sxs-lookup"><span data-stu-id="b0563-130">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="b0563-131">Maximale Größe dieser Auflistung ist 1000 Zeichenfolgen.</span><span class="sxs-lookup"><span data-stu-id="b0563-131">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="b0563-132">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="b0563-132">sourceIdType</span></span> | <span data-ttu-id="b0563-133">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="b0563-133">exchangeIdFormat</span></span> | <span data-ttu-id="b0563-134">Die ID-Typ der Bezeichner in der `InputIds` Parameter.</span><span class="sxs-lookup"><span data-stu-id="b0563-134">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="b0563-135">targetIdType</span><span class="sxs-lookup"><span data-stu-id="b0563-135">targetIdType</span></span> | <span data-ttu-id="b0563-136">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="b0563-136">exchangeIdFormat</span></span> | <span data-ttu-id="b0563-137">Der angeforderte ID-Typ zu konvertieren.</span><span class="sxs-lookup"><span data-stu-id="b0563-137">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="b0563-138">ExchangeIdFormat Werte</span><span class="sxs-lookup"><span data-stu-id="b0563-138">exchangeIdFormat values</span></span>

| <span data-ttu-id="b0563-139">Werte</span><span class="sxs-lookup"><span data-stu-id="b0563-139">Values</span></span> | <span data-ttu-id="b0563-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0563-140">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="b0563-141">entryId</span><span class="sxs-lookup"><span data-stu-id="b0563-141">entryId</span></span> | <span data-ttu-id="b0563-142">Das Format von binären Eintrag ID von MAPI-Clients verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="b0563-142">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="b0563-143">ewsId</span><span class="sxs-lookup"><span data-stu-id="b0563-143">ewsId</span></span> | <span data-ttu-id="b0563-144">Das ID-Format wird von Exchange-Webdienste-Clients verwendet.</span><span class="sxs-lookup"><span data-stu-id="b0563-144">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="b0563-145">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="b0563-145">immutableEntryId</span></span> | <span data-ttu-id="b0563-146">Die MAPI-kompatibles unveränderlich ID Binärformat.</span><span class="sxs-lookup"><span data-stu-id="b0563-146">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="b0563-147">restId</span><span class="sxs-lookup"><span data-stu-id="b0563-147">restId</span></span> | <span data-ttu-id="b0563-148">Das ID-Standardformat, von Microsoft Graph verwendet.</span><span class="sxs-lookup"><span data-stu-id="b0563-148">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="b0563-149">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="b0563-149">restImmutableEntryId</span></span> | <span data-ttu-id="b0563-150">Unveränderlich ID Format wird von Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b0563-150">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="b0563-151">Die binären Dateiformate (`entryId` und `immutableEntryId`) base64-codierte URL-sichere sind.</span><span class="sxs-lookup"><span data-stu-id="b0563-151">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="b0563-152">URL-Safeness wird durch Ändern der base64-Codierung binäre Daten auf folgende Weise implementiert:</span><span class="sxs-lookup"><span data-stu-id="b0563-152">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="b0563-153">Ersetzen Sie `+` mit`-`</span><span class="sxs-lookup"><span data-stu-id="b0563-153">Replace `+` with `-`</span></span>
- <span data-ttu-id="b0563-154">Ersetzen Sie `/` mit`_`</span><span class="sxs-lookup"><span data-stu-id="b0563-154">Replace `/` with `_`</span></span>
- <span data-ttu-id="b0563-155">Entfernen Sie alle nachfolgenden Füllzeichen (`=`)</span><span class="sxs-lookup"><span data-stu-id="b0563-155">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="b0563-156">Eine ganze Zahl an das Ende der Zeichenfolge, die angibt, wie viele Füllzeichen aus der ursprünglichen Datei hinzufügen (`0`, `1`, oder `2`)</span><span class="sxs-lookup"><span data-stu-id="b0563-156">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="b0563-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0563-157">Response</span></span>

<span data-ttu-id="b0563-158">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und eine [ConvertIdResult](../resources/convertidresult.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b0563-158">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0563-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b0563-159">Example</span></span>

<span data-ttu-id="b0563-160">Das folgende Beispiel zeigt, wie mehrere Bezeichner der REST-API-Standardformat konvertiert (`restId`) in das unveränderlich REST-Format (`restImmutableEntryId`).</span><span class="sxs-lookup"><span data-stu-id="b0563-160">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="b0563-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0563-161">Request</span></span>

<span data-ttu-id="b0563-162">Hier sehen Sie die Beispielanforderung:</span><span class="sxs-lookup"><span data-stu-id="b0563-162">Here is the example request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_translateexchangeids"
}-->

```http
POST https://graph.microsoft.com/beta/me/translateExchangeIds
Content-Type: application/json

{
  "inputIds" : [
    "{rest-formatted-id-1}",
    "{rest-formatted-id-2}"
  ],
  "sourceIdType": "restId",
  "targetIdType": "restImmutableEntryId"
}
```

### <a name="response"></a><span data-ttu-id="b0563-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0563-163">Response</span></span>

<span data-ttu-id="b0563-164">Nachfolgend finden Sie die Beispielantwort</span><span class="sxs-lookup"><span data-stu-id="b0563-164">Here is the example response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.convertIdResult",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/testexchangebeta/$metadata#Collection(microsoft.graph.convertIdResult)",
  "value": [
    {
      "sourceId": "{rest-formatted-id-1}",
      "targetId": "{rest-immutable-formatted-id-1}"
    },
    {
      "sourceId": "{rest-formatted-id-2}",
      "targetId": "{rest-immutable-formatted-id-2}"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
