---
title: Vereinbarung erstellen
description: Erstellen eines neuen Vereinbarung-Objekts.
localization_priority: Normal
ms.openlocfilehash: 5040651e032a4f5d0ef2340646f11eb51bfff5eb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514425"
---
# <a name="create-agreement"></a><span data-ttu-id="812fe-103">Vereinbarung erstellen</span><span class="sxs-lookup"><span data-stu-id="812fe-103">Create agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="812fe-104">Erstellen eines neuen [Vereinbarung](../resources/agreement.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="812fe-104">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="812fe-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="812fe-105">Permissions</span></span>
<span data-ttu-id="812fe-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="812fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="812fe-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="812fe-108">Permission type</span></span>                        | <span data-ttu-id="812fe-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="812fe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="812fe-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="812fe-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="812fe-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="812fe-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="812fe-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="812fe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="812fe-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="812fe-113">Not supported.</span></span> |
|<span data-ttu-id="812fe-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="812fe-114">Application</span></span>                            | <span data-ttu-id="812fe-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="812fe-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="812fe-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="812fe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /agreements
```
## <a name="request-headers"></a><span data-ttu-id="812fe-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="812fe-117">Request headers</span></span>
| <span data-ttu-id="812fe-118">Name</span><span class="sxs-lookup"><span data-stu-id="812fe-118">Name</span></span>         | <span data-ttu-id="812fe-119">Typ</span><span class="sxs-lookup"><span data-stu-id="812fe-119">Type</span></span>        | <span data-ttu-id="812fe-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="812fe-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="812fe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="812fe-121">Authorization</span></span> | <span data-ttu-id="812fe-122">string</span><span class="sxs-lookup"><span data-stu-id="812fe-122">string</span></span> | <span data-ttu-id="812fe-123">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="812fe-123">Bearer \{token\}.</span></span> <span data-ttu-id="812fe-124">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="812fe-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="812fe-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="812fe-125">Request body</span></span>
<span data-ttu-id="812fe-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Vertrags](../resources/agreement.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="812fe-126">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="812fe-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen eines Benutzers erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="812fe-127">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="812fe-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="812fe-128">Property</span></span>     | <span data-ttu-id="812fe-129">Typ</span><span class="sxs-lookup"><span data-stu-id="812fe-129">Type</span></span>        | <span data-ttu-id="812fe-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="812fe-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="812fe-131">displayName</span><span class="sxs-lookup"><span data-stu-id="812fe-131">displayName</span></span>|<span data-ttu-id="812fe-132">String</span><span class="sxs-lookup"><span data-stu-id="812fe-132">String</span></span>|<span data-ttu-id="812fe-133">Der Anzeigename der Vereinbarung.</span><span class="sxs-lookup"><span data-stu-id="812fe-133">Display name of the agreement.</span></span>|
|<span data-ttu-id="812fe-134">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="812fe-134">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="812fe-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="812fe-135">Boolean</span></span>|<span data-ttu-id="812fe-136">Gibt an, ob der Benutzer zu erweitern und vor dem akzeptieren die Vereinbarung anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="812fe-136">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="812fe-137">Dateien/fileName</span><span class="sxs-lookup"><span data-stu-id="812fe-137">files/fileName</span></span>|<span data-ttu-id="812fe-138">String</span><span class="sxs-lookup"><span data-stu-id="812fe-138">String</span></span>|<span data-ttu-id="812fe-139">Name der Datei Vereinbarung (beispielsweise TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="812fe-139">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="812fe-140">Dateien/isDefault</span><span class="sxs-lookup"><span data-stu-id="812fe-140">files/isDefault</span></span>|<span data-ttu-id="812fe-141">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="812fe-141">Boolean</span></span>|<span data-ttu-id="812fe-142">Gibt an, ob dies Vereinbarung Standarddatei ist, wenn keiner der Kultur die Client-Vorgabe übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="812fe-142">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="812fe-143">Wenn keine der Datei als Standard angegeben ist, wird der ersten als Standard behandelt.</span><span class="sxs-lookup"><span data-stu-id="812fe-143">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="812fe-144">Dateien/Sprache</span><span class="sxs-lookup"><span data-stu-id="812fe-144">files/language</span></span>|<span data-ttu-id="812fe-145">String</span><span class="sxs-lookup"><span data-stu-id="812fe-145">String</span></span>|<span data-ttu-id="812fe-146">Kultur der Vereinbarung Datei im Format languagecode2-Land/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="812fe-146">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="812fe-147">languagecode2 ist eine zwei-Code aus Kleinbuchstaben ISO 639-1 abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="812fe-147">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="812fe-148">Land/regioncode2 ISO 3166 abgeleitet ist und in der Regel besteht aus zwei Großbuchstaben oder ein Sprachtag BCP 47 (z. B. En-US).</span><span class="sxs-lookup"><span data-stu-id="812fe-148">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="812fe-149">Dateien/FileData/data</span><span class="sxs-lookup"><span data-stu-id="812fe-149">files/fileData/data</span></span>|<span data-ttu-id="812fe-150">Binär</span><span class="sxs-lookup"><span data-stu-id="812fe-150">Binary</span></span>|<span data-ttu-id="812fe-151">Daten, die rechtliche Hinweise das PDF-Dokument darstellt.</span><span class="sxs-lookup"><span data-stu-id="812fe-151">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="812fe-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="812fe-152">Response</span></span>
<span data-ttu-id="812fe-153">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `201, Created` Antwortobjekt Code und [Vereinbarung](../resources/agreement.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="812fe-153">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="812fe-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="812fe-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="812fe-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="812fe-155">Request</span></span>
<span data-ttu-id="812fe-156">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Vertrags](../resources/agreement.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="812fe-156">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="812fe-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="812fe-157">Response</span></span>
><span data-ttu-id="812fe-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="812fe-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-post-agreements.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
