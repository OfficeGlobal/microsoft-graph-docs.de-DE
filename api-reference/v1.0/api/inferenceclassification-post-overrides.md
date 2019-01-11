---
title: inferenceClassificationOverride erstellen
description: 'Erstellen einer Außerkraftsetzung für eine SMTP-Adresse identifizierten Absender. Zukünftige Nachrichten von dieser SMTP-Adresse werden konsistent klassifiziert werden '
localization_priority: Normal
ms.openlocfilehash: 37648d699d4d54b2995af6bf847347c6537a414d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848692"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="1de25-104">inferenceClassificationOverride erstellen</span><span class="sxs-lookup"><span data-stu-id="1de25-104">Create inferenceClassificationOverride</span></span>

<span data-ttu-id="1de25-p102">Erstellen einer Außerkraftsetzung für einen Absender, der durch eine SMTP-Adresse identifiziert wird. Künftige Nachrichten von dieser SMTP-Adresse werden durchgängig klassifiziert wie in der Außerkraftsetzung angegeben.</span><span class="sxs-lookup"><span data-stu-id="1de25-p102">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="1de25-107">**Hinweis**</span><span class="sxs-lookup"><span data-stu-id="1de25-107">**Note**</span></span>

- <span data-ttu-id="1de25-108">Wenn eine Außerkraftsetzung mit der gleichen SMTP-Adresse, bereits vorhanden ist und dann die **ClassifyAs** und **Namen** Felder für die Außerkraftsetzung mit den bereitgestellten Werten aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="1de25-108">If an override already exists with the same STMP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="1de25-109">Die maximale Anzahl von Überschreibungen, die für ein Postfach unterstützt werden, ist 1000, basierend bestimmten SMTP-Absenderadressen.</span><span class="sxs-lookup"><span data-stu-id="1de25-109">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="1de25-110">Im Rahmen des POST-Vorgangs kann immer nur eine Außerkraftsetzung gleichzeitig definiert werden.</span><span class="sxs-lookup"><span data-stu-id="1de25-110">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="1de25-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1de25-111">Permissions</span></span>
<span data-ttu-id="1de25-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1de25-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1de25-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1de25-114">Permission type</span></span>      | <span data-ttu-id="1de25-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1de25-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1de25-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1de25-116">Delegated (work or school account)</span></span> | <span data-ttu-id="1de25-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1de25-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1de25-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1de25-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1de25-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1de25-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1de25-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1de25-120">Application</span></span> | <span data-ttu-id="1de25-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1de25-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1de25-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1de25-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="1de25-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1de25-123">Request headers</span></span>
| <span data-ttu-id="1de25-124">Name</span><span class="sxs-lookup"><span data-stu-id="1de25-124">Name</span></span>       | <span data-ttu-id="1de25-125">Typ</span><span class="sxs-lookup"><span data-stu-id="1de25-125">Type</span></span> | <span data-ttu-id="1de25-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1de25-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1de25-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="1de25-127">Authorization</span></span>  | <span data-ttu-id="1de25-128">string</span><span class="sxs-lookup"><span data-stu-id="1de25-128">string</span></span>  | <span data-ttu-id="1de25-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1de25-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1de25-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1de25-131">Content-Type</span></span> | <span data-ttu-id="1de25-132">string</span><span class="sxs-lookup"><span data-stu-id="1de25-132">string</span></span>  | <span data-ttu-id="1de25-p105">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1de25-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1de25-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1de25-135">Request body</span></span>
<span data-ttu-id="1de25-136">Geben Sie im Anforderungstext eine JSON-Darstellung des [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="1de25-136">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1de25-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="1de25-137">Response</span></span>

<span data-ttu-id="1de25-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1de25-138">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1de25-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1de25-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1de25-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1de25-140">Request</span></span>
<span data-ttu-id="1de25-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1de25-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_inferenceclassificationoverride_from_inferenceclassification"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  }
}
```

##### <a name="response"></a><span data-ttu-id="1de25-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="1de25-142">Response</span></span>
<span data-ttu-id="1de25-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1de25-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
