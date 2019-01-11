---
title: 'Benutzer: TranslateExchangeIds'
description: Übersetzen Sie IDs von Outlook-bezogene Ressourcen zwischen den Formaten.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: b59cc33765586648432736df6067e6c089318729
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831906"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="608c5-103">Benutzer: TranslateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="608c5-103">user: translateExchangeIds</span></span>

> <span data-ttu-id="608c5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="608c5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="608c5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="608c5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="608c5-106">Übersetzen Sie IDs von Outlook-bezogene Ressourcen zwischen den Formaten.</span><span class="sxs-lookup"><span data-stu-id="608c5-106">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="608c5-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="608c5-107">Permissions</span></span>

<span data-ttu-id="608c5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="608c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="608c5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="608c5-110">Permission type</span></span> | <span data-ttu-id="608c5-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="608c5-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="608c5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="608c5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="608c5-113">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="608c5-113">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="608c5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="608c5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="608c5-115">User.ReadBasic, User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="608c5-115">User.ReadBasic, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="608c5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="608c5-116">Application</span></span> | <span data-ttu-id="608c5-117">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="608c5-117">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="608c5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="608c5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="608c5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="608c5-119">Request headers</span></span>

| <span data-ttu-id="608c5-120">Name</span><span class="sxs-lookup"><span data-stu-id="608c5-120">Name</span></span> | <span data-ttu-id="608c5-121">Wert</span><span class="sxs-lookup"><span data-stu-id="608c5-121">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="608c5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="608c5-122">Authorization</span></span> | <span data-ttu-id="608c5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="608c5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="608c5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="608c5-125">Request body</span></span>

| <span data-ttu-id="608c5-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="608c5-126">Parameter</span></span> | <span data-ttu-id="608c5-127">Typ</span><span class="sxs-lookup"><span data-stu-id="608c5-127">Type</span></span> | <span data-ttu-id="608c5-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="608c5-128">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="608c5-129">inputIds</span><span class="sxs-lookup"><span data-stu-id="608c5-129">inputIds</span></span> | <span data-ttu-id="608c5-130">Edm.String-Auflistung</span><span class="sxs-lookup"><span data-stu-id="608c5-130">Edm.String collection</span></span> | <span data-ttu-id="608c5-131">Eine Sammlung von Bezeichnern zu konvertieren.</span><span class="sxs-lookup"><span data-stu-id="608c5-131">A collection of identifiers to convert.</span></span> <span data-ttu-id="608c5-132">Alle Bezeichner in der Auflistung der gleichen ID Quelltyp benötigen und für Elemente im selben Postfach werden müssen.</span><span class="sxs-lookup"><span data-stu-id="608c5-132">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="608c5-133">Maximale Größe dieser Auflistung ist 1000 Zeichenfolgen.</span><span class="sxs-lookup"><span data-stu-id="608c5-133">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="608c5-134">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="608c5-134">sourceIdType</span></span> | <span data-ttu-id="608c5-135">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="608c5-135">exchangeIdFormat</span></span> | <span data-ttu-id="608c5-136">Die ID-Typ der Bezeichner in der `InputIds` Parameter.</span><span class="sxs-lookup"><span data-stu-id="608c5-136">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="608c5-137">targetIdType</span><span class="sxs-lookup"><span data-stu-id="608c5-137">targetIdType</span></span> | <span data-ttu-id="608c5-138">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="608c5-138">exchangeIdFormat</span></span> | <span data-ttu-id="608c5-139">Der angeforderte ID-Typ zu konvertieren.</span><span class="sxs-lookup"><span data-stu-id="608c5-139">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="608c5-140">ExchangeIdFormat Werte</span><span class="sxs-lookup"><span data-stu-id="608c5-140">exchangeIdFormat values</span></span>

| <span data-ttu-id="608c5-141">Werte</span><span class="sxs-lookup"><span data-stu-id="608c5-141">Values</span></span> | <span data-ttu-id="608c5-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="608c5-142">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="608c5-143">entryId</span><span class="sxs-lookup"><span data-stu-id="608c5-143">entryId</span></span> | <span data-ttu-id="608c5-144">Das Format von binären Eintrag ID von MAPI-Clients verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="608c5-144">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="608c5-145">ewsId</span><span class="sxs-lookup"><span data-stu-id="608c5-145">ewsId</span></span> | <span data-ttu-id="608c5-146">Das ID-Format wird von Exchange-Webdienste-Clients verwendet.</span><span class="sxs-lookup"><span data-stu-id="608c5-146">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="608c5-147">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="608c5-147">immutableEntryId</span></span> | <span data-ttu-id="608c5-148">Die MAPI-kompatibles unveränderlich ID Binärformat.</span><span class="sxs-lookup"><span data-stu-id="608c5-148">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="608c5-149">restId</span><span class="sxs-lookup"><span data-stu-id="608c5-149">restId</span></span> | <span data-ttu-id="608c5-150">Das ID-Standardformat, von Microsoft Graph verwendet.</span><span class="sxs-lookup"><span data-stu-id="608c5-150">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="608c5-151">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="608c5-151">restImmutableEntryId</span></span> | <span data-ttu-id="608c5-152">Unveränderlich ID Format wird von Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="608c5-152">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="608c5-153">Die binären Dateiformate (`entryId` und `immutableEntryId`) base64-codierte URL-sichere sind.</span><span class="sxs-lookup"><span data-stu-id="608c5-153">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="608c5-154">URL-Safeness wird durch Ändern der base64-Codierung binäre Daten auf folgende Weise implementiert:</span><span class="sxs-lookup"><span data-stu-id="608c5-154">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="608c5-155">Ersetzen Sie `+` mit`-`</span><span class="sxs-lookup"><span data-stu-id="608c5-155">Replace `+` with `-`</span></span>
- <span data-ttu-id="608c5-156">Ersetzen Sie `/` mit`_`</span><span class="sxs-lookup"><span data-stu-id="608c5-156">Replace `/` with `_`</span></span>
- <span data-ttu-id="608c5-157">Entfernen Sie alle nachfolgenden Füllzeichen (`=`)</span><span class="sxs-lookup"><span data-stu-id="608c5-157">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="608c5-158">Eine ganze Zahl an das Ende der Zeichenfolge, die angibt, wie viele Füllzeichen aus der ursprünglichen Datei hinzufügen (`0`, `1`, oder `2`)</span><span class="sxs-lookup"><span data-stu-id="608c5-158">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="608c5-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="608c5-159">Response</span></span>

<span data-ttu-id="608c5-160">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und eine [ConvertIdResult](../resources/convertidresult.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="608c5-160">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="608c5-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="608c5-161">Example</span></span>

<span data-ttu-id="608c5-162">Das folgende Beispiel zeigt, wie mehrere Bezeichner der REST-API-Standardformat konvertiert (`restId`) in das unveränderlich REST-Format (`restImmutableEntryId`).</span><span class="sxs-lookup"><span data-stu-id="608c5-162">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="608c5-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="608c5-163">Request</span></span>

<span data-ttu-id="608c5-164">Hier sehen Sie die Beispielanforderung:</span><span class="sxs-lookup"><span data-stu-id="608c5-164">Here is the example request.</span></span>
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

### <a name="response"></a><span data-ttu-id="608c5-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="608c5-165">Response</span></span>

<span data-ttu-id="608c5-166">Nachfolgend finden Sie die Beispielantwort</span><span class="sxs-lookup"><span data-stu-id="608c5-166">Here is the example response</span></span>
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
      "sourceId": "{rest-formatted-id-1},
      "targetId": "{rest-immutable-formatted-id-1}"
    },
    {
      "sourceId": "{rest-formatted-id-2},
      "targetId": "{rest-immutable-formatted-id-2}"
    }
  ]
}
```
