---
title: inferenceClassificationOverride erstellen
description: 'Erstellen Sie eine praxisorientierte Posteingang Überschreibung für eine SMTP-Adresse identifizierten Absender. Zukünftige Nachrichten von dieser SMTP-Adresse werden konsistent klassifiziert werden '
localization_priority: Normal
ms.openlocfilehash: 234972bea59343a13d9104bbe222edf4be526987
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516119"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="ebb71-104">inferenceClassificationOverride erstellen</span><span class="sxs-lookup"><span data-stu-id="ebb71-104">Create inferenceClassificationOverride</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebb71-105">Erstellen Sie eine [Praxisorientierte Posteingang](../resources/manage-focused-inbox.md) Überschreibung für eine SMTP-Adresse identifizierten Absender.</span><span class="sxs-lookup"><span data-stu-id="ebb71-105">Create a [Focused Inbox](../resources/manage-focused-inbox.md) override for a sender identified by an SMTP address.</span></span> <span data-ttu-id="ebb71-106">Nachrichten von diesem SMTP-Adresse konsistent eingestuft wird wie in die Außerkraftsetzung angegeben.</span><span class="sxs-lookup"><span data-stu-id="ebb71-106">Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="ebb71-107">**Hinweis**</span><span class="sxs-lookup"><span data-stu-id="ebb71-107">**Note**</span></span>

- <span data-ttu-id="ebb71-108">Wenn eine Außerkraftsetzung mit der gleichen SMTP-Adresse, bereits vorhanden ist und dann die **ClassifyAs** und **Namen** Felder für die Außerkraftsetzung mit den bereitgestellten Werten aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="ebb71-108">If an override already exists with the same STMP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="ebb71-109">Die maximale Anzahl von Überschreibungen, die für ein Postfach unterstützt werden, ist 1000, basierend bestimmten SMTP-Absenderadressen.</span><span class="sxs-lookup"><span data-stu-id="ebb71-109">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="ebb71-110">Im Rahmen des POST-Vorgangs kann immer nur eine Außerkraftsetzung gleichzeitig definiert werden.</span><span class="sxs-lookup"><span data-stu-id="ebb71-110">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebb71-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ebb71-111">Permissions</span></span>
<span data-ttu-id="ebb71-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebb71-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebb71-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ebb71-114">Permission type</span></span>      | <span data-ttu-id="ebb71-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ebb71-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebb71-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ebb71-116">Delegated (work or school account)</span></span> | <span data-ttu-id="ebb71-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebb71-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ebb71-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ebb71-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebb71-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebb71-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ebb71-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ebb71-120">Application</span></span> | <span data-ttu-id="ebb71-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebb71-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebb71-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ebb71-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="ebb71-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ebb71-123">Request headers</span></span>
| <span data-ttu-id="ebb71-124">Name</span><span class="sxs-lookup"><span data-stu-id="ebb71-124">Name</span></span>       | <span data-ttu-id="ebb71-125">Typ</span><span class="sxs-lookup"><span data-stu-id="ebb71-125">Type</span></span> | <span data-ttu-id="ebb71-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ebb71-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ebb71-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebb71-127">Authorization</span></span>  | <span data-ttu-id="ebb71-128">string</span><span class="sxs-lookup"><span data-stu-id="ebb71-128">string</span></span>  | <span data-ttu-id="ebb71-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ebb71-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ebb71-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ebb71-131">Content-Type</span></span> | <span data-ttu-id="ebb71-132">string</span><span class="sxs-lookup"><span data-stu-id="ebb71-132">string</span></span>  | <span data-ttu-id="ebb71-p105">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ebb71-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ebb71-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ebb71-135">Request body</span></span>
<span data-ttu-id="ebb71-136">Geben Sie im Anforderungstext eine JSON-Darstellung des [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ebb71-136">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ebb71-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="ebb71-137">Response</span></span>

<span data-ttu-id="ebb71-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ebb71-138">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebb71-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ebb71-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebb71-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ebb71-140">Request</span></span>
<span data-ttu-id="ebb71-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ebb71-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_inferenceclassificationoverride_from_inferenceclassification"
}-->
```http
POST https://graph.microsoft.com/beta/me/inferenceClassification/overrides
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  }
}
```

##### <a name="response"></a><span data-ttu-id="ebb71-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="ebb71-142">Response</span></span>
<span data-ttu-id="ebb71-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ebb71-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/inferenceclassification-post-overrides.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
