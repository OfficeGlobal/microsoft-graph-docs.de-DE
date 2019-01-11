---
title: InferenceClassificationOverride aktualisieren
description: 'Ändern Sie das Feld **ClassifyAs** eine praxisorientierte Posteingang außer Kraft setzen, wie angegeben. '
localization_priority: Normal
ms.openlocfilehash: b9d462bc09f69b07d5b6b4bce031932e1b702b44
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887905"
---
# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="c6cb5-103">InferenceClassificationOverride aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c6cb5-103">Update inferenceClassificationOverride</span></span>

> <span data-ttu-id="c6cb5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c6cb5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6cb5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c6cb5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c6cb5-106">Ändern Sie das Feld **ClassifyAs** eine [Praxisorientierte Posteingang](../resources/manage-focused-inbox.md) außer Kraft setzen, wie angegeben.</span><span class="sxs-lookup"><span data-stu-id="c6cb5-106">Change the **classifyAs** field of a [Focused Inbox](../resources/manage-focused-inbox.md) override as specified.</span></span> 

<span data-ttu-id="c6cb5-107">Sie können PATCH nicht zum Ändern von anderen Feldern in einer [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)-Instanz verwenden.</span><span class="sxs-lookup"><span data-stu-id="c6cb5-107">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) instance.</span></span> 

<span data-ttu-id="c6cb5-108">Wenn eine Außerkraftsetzung für einen Absender vorhanden ist und der Absender den Anzeigenamen ändert, können Sie [POST](inferenceclassification-post-overrides.md) zum Erzwingen einer Aktualisierung des Namensfelds in der vorhandenen Außerkraftsetzung verwenden.</span><span class="sxs-lookup"><span data-stu-id="c6cb5-108">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification-post-overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="c6cb5-109">Wenn eine Außerkraftsetzung für einen Absender vorhanden ist und der Absender die SMTP-Adresse ändert, können Sie die Außerkraftsetzung für diesen Absender nur „aktualisieren“, indem Sie die vorhandene Außerkraftsetzung [löschen](inferenceclassificationoverride-delete.md) und eine neue Außerkraftsetzung mit der neuen SMTP-Adresse [erstellen](inferenceclassification-post-overrides.md).</span><span class="sxs-lookup"><span data-stu-id="c6cb5-109">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride-delete.md) the existing override and [creating](inferenceclassification-post-overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6cb5-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c6cb5-110">Permissions</span></span>
<span data-ttu-id="c6cb5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6cb5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6cb5-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c6cb5-113">Permission type</span></span>      | <span data-ttu-id="c6cb5-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c6cb5-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6cb5-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c6cb5-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c6cb5-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6cb5-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c6cb5-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c6cb5-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6cb5-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6cb5-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c6cb5-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c6cb5-119">Application</span></span> | <span data-ttu-id="c6cb5-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6cb5-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6cb5-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c6cb5-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c6cb5-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c6cb5-122">Request headers</span></span>
| <span data-ttu-id="c6cb5-123">Name</span><span class="sxs-lookup"><span data-stu-id="c6cb5-123">Name</span></span>       | <span data-ttu-id="c6cb5-124">Typ</span><span class="sxs-lookup"><span data-stu-id="c6cb5-124">Type</span></span> | <span data-ttu-id="c6cb5-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6cb5-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c6cb5-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6cb5-126">Authorization</span></span>  | <span data-ttu-id="c6cb5-127">string</span><span class="sxs-lookup"><span data-stu-id="c6cb5-127">string</span></span>  | <span data-ttu-id="c6cb5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c6cb5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c6cb5-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c6cb5-130">Content-Type</span></span> | <span data-ttu-id="c6cb5-131">string</span><span class="sxs-lookup"><span data-stu-id="c6cb5-131">string</span></span>  | <span data-ttu-id="c6cb5-p104">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c6cb5-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6cb5-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c6cb5-134">Request body</span></span>
<span data-ttu-id="c6cb5-p105">Geben Sie im Anforderungstext den neuen Wert für **classifyAs** an. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="c6cb5-p105">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="c6cb5-137">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c6cb5-137">Property</span></span>     | <span data-ttu-id="c6cb5-138">Typ</span><span class="sxs-lookup"><span data-stu-id="c6cb5-138">Type</span></span>   |<span data-ttu-id="c6cb5-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6cb5-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6cb5-140">classifyAs</span><span class="sxs-lookup"><span data-stu-id="c6cb5-140">classifyAs</span></span>|<span data-ttu-id="c6cb5-141">string</span><span class="sxs-lookup"><span data-stu-id="c6cb5-141">string</span></span>| <span data-ttu-id="c6cb5-p106">Gibt an, wie eingehende Nachrichten von einem bestimmten Absender immer klassifiziert werden sollen. Mögliche Werte: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="c6cb5-p106">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="c6cb5-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="c6cb5-144">Response</span></span>

<span data-ttu-id="c6cb5-145">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c6cb5-145">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c6cb5-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c6cb5-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6cb5-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c6cb5-147">Request</span></span>
<span data-ttu-id="c6cb5-148">Im folgenden Beispiel wird die Außerkraftsetzung für die SMTP-Adresse „randiw@adatum.onmicrosoft.com“ von `other` zu `focused` geändert.</span><span class="sxs-lookup"><span data-stu-id="c6cb5-148">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_inferenceclassificationoverride"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/inferenceClassification/overrides/{id}
Content-type: application/json

{
  "classifyAs": "focused"
}
```
##### <a name="response"></a><span data-ttu-id="c6cb5-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="c6cb5-149">Response</span></span>
<span data-ttu-id="c6cb5-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c6cb5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
