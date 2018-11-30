---
title: inferenceClassificationOverride erstellen
description: 'Erstellen Sie eine praxisorientierte Posteingang Überschreibung für eine SMTP-Adresse identifizierten Absender. Zukünftige Nachrichten von dieser SMTP-Adresse werden konsistent klassifiziert werden '
ms.openlocfilehash: e15793bc8c7012628659144bd503bd8cf979ef61
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060931"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="73e98-104">inferenceClassificationOverride erstellen</span><span class="sxs-lookup"><span data-stu-id="73e98-104">Create inferenceClassificationOverride</span></span>

> <span data-ttu-id="73e98-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="73e98-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73e98-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="73e98-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="73e98-107">Erstellen Sie eine [Praxisorientierte Posteingang](../resources/manage-focused-inbox.md) Überschreibung für eine SMTP-Adresse identifizierten Absender.</span><span class="sxs-lookup"><span data-stu-id="73e98-107">Create a [Focused Inbox](../resources/manage-focused-inbox.md) override for a sender identified by an SMTP address.</span></span> <span data-ttu-id="73e98-108">Nachrichten von diesem SMTP-Adresse konsistent eingestuft wird wie in die Außerkraftsetzung angegeben.</span><span class="sxs-lookup"><span data-stu-id="73e98-108">Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="73e98-109">**Hinweis**</span><span class="sxs-lookup"><span data-stu-id="73e98-109">**Note**</span></span>

- <span data-ttu-id="73e98-110">Wenn eine Außerkraftsetzung mit der gleichen SMTP-Adresse, bereits vorhanden ist und dann die **ClassifyAs** und **Namen** Felder für die Außerkraftsetzung mit den bereitgestellten Werten aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="73e98-110">If an override already exists with the same STMP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="73e98-111">Die maximale Anzahl von Überschreibungen, die für ein Postfach unterstützt werden, ist 1000, basierend bestimmten SMTP-Absenderadressen.</span><span class="sxs-lookup"><span data-stu-id="73e98-111">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="73e98-112">Im Rahmen des POST-Vorgangs kann immer nur eine Außerkraftsetzung gleichzeitig definiert werden.</span><span class="sxs-lookup"><span data-stu-id="73e98-112">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="73e98-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="73e98-113">Permissions</span></span>
<span data-ttu-id="73e98-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73e98-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73e98-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="73e98-116">Permission type</span></span>      | <span data-ttu-id="73e98-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="73e98-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73e98-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="73e98-118">Delegated (work or school account)</span></span> | <span data-ttu-id="73e98-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73e98-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="73e98-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="73e98-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73e98-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73e98-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="73e98-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="73e98-122">Application</span></span> | <span data-ttu-id="73e98-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73e98-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="73e98-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="73e98-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="73e98-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="73e98-125">Request headers</span></span>
| <span data-ttu-id="73e98-126">Name</span><span class="sxs-lookup"><span data-stu-id="73e98-126">Name</span></span>       | <span data-ttu-id="73e98-127">Typ</span><span class="sxs-lookup"><span data-stu-id="73e98-127">Type</span></span> | <span data-ttu-id="73e98-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73e98-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="73e98-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="73e98-129">Authorization</span></span>  | <span data-ttu-id="73e98-130">string</span><span class="sxs-lookup"><span data-stu-id="73e98-130">string</span></span>  | <span data-ttu-id="73e98-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="73e98-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="73e98-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73e98-133">Content-Type</span></span> | <span data-ttu-id="73e98-134">string</span><span class="sxs-lookup"><span data-stu-id="73e98-134">string</span></span>  | <span data-ttu-id="73e98-p106">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="73e98-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73e98-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="73e98-137">Request body</span></span>
<span data-ttu-id="73e98-138">Geben Sie im Anforderungstext eine JSON-Darstellung des [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="73e98-138">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="73e98-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="73e98-139">Response</span></span>

<span data-ttu-id="73e98-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73e98-140">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73e98-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="73e98-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73e98-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="73e98-142">Request</span></span>
<span data-ttu-id="73e98-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="73e98-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="73e98-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="73e98-144">Response</span></span>
<span data-ttu-id="73e98-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73e98-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->