---
title: Vereinbarung erstellen
description: Erstellen eines neuen Vereinbarung-Objekts.
localization_priority: Normal
ms.openlocfilehash: 4768912a7c5be722878d6b910d6d68ded460c702
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870637"
---
# <a name="create-agreement"></a><span data-ttu-id="f4e57-103">Vereinbarung erstellen</span><span class="sxs-lookup"><span data-stu-id="f4e57-103">Create agreement</span></span>

> <span data-ttu-id="f4e57-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f4e57-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f4e57-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f4e57-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f4e57-106">Erstellen eines neuen [Vereinbarung](../resources/agreement.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f4e57-106">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f4e57-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f4e57-107">Permissions</span></span>
<span data-ttu-id="f4e57-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4e57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4e57-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f4e57-110">Permission type</span></span>                        | <span data-ttu-id="f4e57-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f4e57-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4e57-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f4e57-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f4e57-113">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4e57-113">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="f4e57-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f4e57-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4e57-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f4e57-115">Not supported.</span></span> |
|<span data-ttu-id="f4e57-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f4e57-116">Application</span></span>                            | <span data-ttu-id="f4e57-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f4e57-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4e57-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4e57-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /agreements
```
## <a name="request-headers"></a><span data-ttu-id="f4e57-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f4e57-119">Request headers</span></span>
| <span data-ttu-id="f4e57-120">Name</span><span class="sxs-lookup"><span data-stu-id="f4e57-120">Name</span></span>         | <span data-ttu-id="f4e57-121">Typ</span><span class="sxs-lookup"><span data-stu-id="f4e57-121">Type</span></span>        | <span data-ttu-id="f4e57-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4e57-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f4e57-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4e57-123">Authorization</span></span> | <span data-ttu-id="f4e57-124">string</span><span class="sxs-lookup"><span data-stu-id="f4e57-124">string</span></span> | <span data-ttu-id="f4e57-125">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="f4e57-125">Bearer \{token\}.</span></span> <span data-ttu-id="f4e57-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f4e57-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4e57-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f4e57-127">Request body</span></span>
<span data-ttu-id="f4e57-128">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Vertrags](../resources/agreement.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f4e57-128">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="f4e57-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen eines Benutzers erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="f4e57-129">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="f4e57-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f4e57-130">Property</span></span>     | <span data-ttu-id="f4e57-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f4e57-131">Type</span></span>        | <span data-ttu-id="f4e57-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4e57-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f4e57-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f4e57-133">displayName</span></span>|<span data-ttu-id="f4e57-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4e57-134">String</span></span>|<span data-ttu-id="f4e57-135">Der Anzeigename der Vereinbarung.</span><span class="sxs-lookup"><span data-stu-id="f4e57-135">Display name of the agreement.</span></span>|
|<span data-ttu-id="f4e57-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="f4e57-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="f4e57-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f4e57-137">Boolean</span></span>|<span data-ttu-id="f4e57-138">Gibt an, ob der Benutzer zu erweitern und vor dem akzeptieren die Vereinbarung anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="f4e57-138">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="f4e57-139">Dateien/fileName</span><span class="sxs-lookup"><span data-stu-id="f4e57-139">files/fileName</span></span>|<span data-ttu-id="f4e57-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4e57-140">String</span></span>|<span data-ttu-id="f4e57-141">Name der Datei Vereinbarung (beispielsweise TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="f4e57-141">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="f4e57-142">Dateien/isDefault</span><span class="sxs-lookup"><span data-stu-id="f4e57-142">files/isDefault</span></span>|<span data-ttu-id="f4e57-143">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f4e57-143">Boolean</span></span>|<span data-ttu-id="f4e57-144">Gibt an, ob dies Vereinbarung Standarddatei ist, wenn keiner der Kultur die Client-Vorgabe übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="f4e57-144">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="f4e57-145">Wenn keine der Datei als Standard angegeben ist, wird der ersten als Standard behandelt.</span><span class="sxs-lookup"><span data-stu-id="f4e57-145">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="f4e57-146">Dateien/Sprache</span><span class="sxs-lookup"><span data-stu-id="f4e57-146">files/language</span></span>|<span data-ttu-id="f4e57-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f4e57-147">String</span></span>|<span data-ttu-id="f4e57-148">Kultur der Vereinbarung Datei im Format languagecode2-Land/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="f4e57-148">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="f4e57-149">languagecode2 ist eine zwei-Code aus Kleinbuchstaben ISO 639-1 abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="f4e57-149">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="f4e57-150">Land/regioncode2 ISO 3166 abgeleitet ist und in der Regel besteht aus zwei Großbuchstaben oder ein Sprachtag BCP 47 (z. B. En-US).</span><span class="sxs-lookup"><span data-stu-id="f4e57-150">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="f4e57-151">Dateien/FileData/data</span><span class="sxs-lookup"><span data-stu-id="f4e57-151">files/fileData/data</span></span>|<span data-ttu-id="f4e57-152">Binär</span><span class="sxs-lookup"><span data-stu-id="f4e57-152">Binary</span></span>|<span data-ttu-id="f4e57-153">Daten, die rechtliche Hinweise das PDF-Dokument darstellt.</span><span class="sxs-lookup"><span data-stu-id="f4e57-153">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="f4e57-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4e57-154">Response</span></span>
<span data-ttu-id="f4e57-155">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `201, Created` Antwortobjekt Code und [Vereinbarung](../resources/agreement.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f4e57-155">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4e57-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f4e57-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f4e57-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4e57-157">Request</span></span>
<span data-ttu-id="f4e57-158">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Vertrags](../resources/agreement.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f4e57-158">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_agreement_from_agreements"
}-->
```http
POST https://graph.microsoft.com/beta/agreements
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "files": [
    {
      "fileName": "TOU.pdf",
      "language": "en",
      "isDefault": true,
      "fileData": {
        "data": "SGVsbG8gd29ybGQ="
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="f4e57-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4e57-159">Response</span></span>
><span data-ttu-id="f4e57-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f4e57-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
