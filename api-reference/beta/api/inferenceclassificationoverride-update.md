---
title: inferenceclassificationoverride aktualisieren
description: 'Ändern Sie das Feld **ClassifyAs** eine praxisorientierte Posteingang außer Kraft setzen, wie angegeben. '
localization_priority: Normal
ms.openlocfilehash: 0cb3eab7f8a4efece8099ca8f65577d8a06b18d6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508517"
---
# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="e96e7-103">inferenceclassificationoverride aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e96e7-103">Update inferenceClassificationOverride</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e96e7-104">Ändern Sie das Feld **ClassifyAs** eine [Praxisorientierte Posteingang](../resources/manage-focused-inbox.md) außer Kraft setzen, wie angegeben.</span><span class="sxs-lookup"><span data-stu-id="e96e7-104">Change the **classifyAs** field of a [Focused Inbox](../resources/manage-focused-inbox.md) override as specified.</span></span> 

<span data-ttu-id="e96e7-105">Sie können PATCH nicht zum Ändern von anderen Feldern in einer [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)-Instanz verwenden.</span><span class="sxs-lookup"><span data-stu-id="e96e7-105">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) instance.</span></span> 

<span data-ttu-id="e96e7-106">Wenn eine Außerkraftsetzung für einen Absender vorhanden ist und der Absender den Anzeigenamen ändert, können Sie [POST](inferenceclassification-post-overrides.md) zum Erzwingen einer Aktualisierung des Namensfelds in der vorhandenen Außerkraftsetzung verwenden.</span><span class="sxs-lookup"><span data-stu-id="e96e7-106">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification-post-overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="e96e7-107">Wenn eine Außerkraftsetzung für einen Absender vorhanden ist und der Absender die SMTP-Adresse ändert, können Sie die Außerkraftsetzung für diesen Absender nur „aktualisieren“, indem Sie die vorhandene Außerkraftsetzung [löschen](inferenceclassificationoverride-delete.md) und eine neue Außerkraftsetzung mit der neuen SMTP-Adresse [erstellen](inferenceclassification-post-overrides.md).</span><span class="sxs-lookup"><span data-stu-id="e96e7-107">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride-delete.md) the existing override and [creating](inferenceclassification-post-overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="e96e7-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e96e7-108">Permissions</span></span>
<span data-ttu-id="e96e7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e96e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e96e7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e96e7-111">Permission type</span></span>      | <span data-ttu-id="e96e7-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e96e7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e96e7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e96e7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e96e7-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e96e7-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e96e7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e96e7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e96e7-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e96e7-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e96e7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e96e7-117">Application</span></span> | <span data-ttu-id="e96e7-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e96e7-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e96e7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e96e7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e96e7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e96e7-120">Request headers</span></span>
| <span data-ttu-id="e96e7-121">Name</span><span class="sxs-lookup"><span data-stu-id="e96e7-121">Name</span></span>       | <span data-ttu-id="e96e7-122">Typ</span><span class="sxs-lookup"><span data-stu-id="e96e7-122">Type</span></span> | <span data-ttu-id="e96e7-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e96e7-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e96e7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e96e7-124">Authorization</span></span>  | <span data-ttu-id="e96e7-125">String</span><span class="sxs-lookup"><span data-stu-id="e96e7-125">string</span></span>  | <span data-ttu-id="e96e7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e96e7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e96e7-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e96e7-128">Content-Type</span></span> | <span data-ttu-id="e96e7-129">string</span><span class="sxs-lookup"><span data-stu-id="e96e7-129">string</span></span>  | <span data-ttu-id="e96e7-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e96e7-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e96e7-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e96e7-132">Request body</span></span>
<span data-ttu-id="e96e7-p104">Geben Sie im Anforderungstext den neuen Wert für **classifyAs** an. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="e96e7-p104">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="e96e7-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e96e7-135">Property</span></span>     | <span data-ttu-id="e96e7-136">Typ</span><span class="sxs-lookup"><span data-stu-id="e96e7-136">Type</span></span>   |<span data-ttu-id="e96e7-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e96e7-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e96e7-138">classifyAs</span><span class="sxs-lookup"><span data-stu-id="e96e7-138">classifyAs</span></span>|<span data-ttu-id="e96e7-139">string</span><span class="sxs-lookup"><span data-stu-id="e96e7-139">string</span></span>| <span data-ttu-id="e96e7-p105">Gibt an, wie eingehende Nachrichten von einem bestimmten Absender immer klassifiziert werden sollen. Mögliche Werte: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="e96e7-p105">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="e96e7-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="e96e7-142">Response</span></span>

<span data-ttu-id="e96e7-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e96e7-143">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e96e7-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e96e7-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e96e7-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e96e7-145">Request</span></span>
<span data-ttu-id="e96e7-146">Im folgenden Beispiel wird die Außerkraftsetzung für die SMTP-Adresse „randiw@adatum.onmicrosoft.com“ von `other` zu `focused` geändert.</span><span class="sxs-lookup"><span data-stu-id="e96e7-146">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>

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
##### <a name="response"></a><span data-ttu-id="e96e7-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="e96e7-147">Response</span></span>
<span data-ttu-id="e96e7-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e96e7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update inferenceclassificationoverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/inferenceclassificationoverride-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
