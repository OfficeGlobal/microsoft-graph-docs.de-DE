---
title: inferenceclassificationoverride aktualisieren
description: 'Ändert das **classifyAs**-Feld einer Außerkraftsetzung wie angegeben. '
localization_priority: Normal
ms.openlocfilehash: fdd11e6c3d3f4fb72d9f94226e8cb3d35dde2c03
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843974"
---
# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="191aa-103">inferenceclassificationoverride aktualisieren</span><span class="sxs-lookup"><span data-stu-id="191aa-103">Update inferenceclassificationoverride</span></span>

<span data-ttu-id="191aa-104">Ändert das **classifyAs**-Feld einer Außerkraftsetzung wie angegeben.</span><span class="sxs-lookup"><span data-stu-id="191aa-104">Change the **classifyAs** field of an override as specified.</span></span> 

<span data-ttu-id="191aa-105">Sie können PATCH nicht zum Ändern von anderen Feldern in einer [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)-Instanz verwenden.</span><span class="sxs-lookup"><span data-stu-id="191aa-105">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) instance.</span></span> 

<span data-ttu-id="191aa-106">Wenn eine Außerkraftsetzung für einen Absender vorhanden ist und der Absender den Anzeigenamen ändert, können Sie [POST](inferenceclassification-post-overrides.md) zum Erzwingen einer Aktualisierung des Namensfelds in der vorhandenen Außerkraftsetzung verwenden.</span><span class="sxs-lookup"><span data-stu-id="191aa-106">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification-post-overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="191aa-107">Wenn eine Außerkraftsetzung für einen Absender vorhanden ist und der Absender die SMTP-Adresse ändert, können Sie die Außerkraftsetzung für diesen Absender nur „aktualisieren“, indem Sie die vorhandene Außerkraftsetzung [löschen](inferenceclassificationoverride-delete.md) und eine neue Außerkraftsetzung mit der neuen SMTP-Adresse [erstellen](inferenceclassification-post-overrides.md).</span><span class="sxs-lookup"><span data-stu-id="191aa-107">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride-delete.md) the existing override and [creating](inferenceclassification-post-overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="191aa-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="191aa-108">Permissions</span></span>
<span data-ttu-id="191aa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="191aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="191aa-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="191aa-111">Permission type</span></span>      | <span data-ttu-id="191aa-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="191aa-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="191aa-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="191aa-113">Delegated (work or school account)</span></span> | <span data-ttu-id="191aa-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="191aa-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="191aa-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="191aa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="191aa-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="191aa-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="191aa-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="191aa-117">Application</span></span> | <span data-ttu-id="191aa-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="191aa-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="191aa-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="191aa-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="191aa-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="191aa-120">Request headers</span></span>
| <span data-ttu-id="191aa-121">Name</span><span class="sxs-lookup"><span data-stu-id="191aa-121">Name</span></span>       | <span data-ttu-id="191aa-122">Typ</span><span class="sxs-lookup"><span data-stu-id="191aa-122">Type</span></span> | <span data-ttu-id="191aa-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="191aa-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="191aa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="191aa-124">Authorization</span></span>  | <span data-ttu-id="191aa-125">string</span><span class="sxs-lookup"><span data-stu-id="191aa-125">string</span></span>  | <span data-ttu-id="191aa-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="191aa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="191aa-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="191aa-128">Content-Type</span></span> | <span data-ttu-id="191aa-129">string</span><span class="sxs-lookup"><span data-stu-id="191aa-129">string</span></span>  | <span data-ttu-id="191aa-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="191aa-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="191aa-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="191aa-132">Request body</span></span>
<span data-ttu-id="191aa-p104">Geben Sie im Anforderungstext den neuen Wert für **classifyAs** an. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="191aa-p104">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="191aa-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="191aa-135">Property</span></span>     | <span data-ttu-id="191aa-136">Typ</span><span class="sxs-lookup"><span data-stu-id="191aa-136">Type</span></span>   |<span data-ttu-id="191aa-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="191aa-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="191aa-138">classifyAs</span><span class="sxs-lookup"><span data-stu-id="191aa-138">classifyAs</span></span>|<span data-ttu-id="191aa-139">string</span><span class="sxs-lookup"><span data-stu-id="191aa-139">string</span></span>| <span data-ttu-id="191aa-140">Gibt an, wie eingehende-Nachrichten von einer bestimmten Absender sollte stets als klassifiziert werden.</span><span class="sxs-lookup"><span data-stu-id="191aa-140">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="191aa-141">Die möglichen Werte sind: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="191aa-141">The possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="191aa-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="191aa-142">Response</span></span>

<span data-ttu-id="191aa-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="191aa-143">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="191aa-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="191aa-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="191aa-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="191aa-145">Request</span></span>
<span data-ttu-id="191aa-146">Im folgenden Beispiel wird die Außerkraftsetzung für die SMTP-Adresse „randiw@adatum.onmicrosoft.com“ von `other` zu `focused` geändert.</span><span class="sxs-lookup"><span data-stu-id="191aa-146">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_inferenceclassificationoverride"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/{id}
Content-type: application/json

{
  "classifyAs": "focused"
}
```
##### <a name="response"></a><span data-ttu-id="191aa-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="191aa-147">Response</span></span>
<span data-ttu-id="191aa-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="191aa-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Randi Welch",
    "address": "randiw@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update inferenceclassificationoverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
