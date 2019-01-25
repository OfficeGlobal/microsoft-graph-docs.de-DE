---
title: Organisation aktualisieren
description: Mit dieser API können Sie die Eigenschaften der aktuell authentifizierten Organisation aktualisieren.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 090be61f98ecd8f55a5e1a9edfe45bf7b39f23de
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526844"
---
# <a name="update-organization"></a><span data-ttu-id="21a81-103">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="21a81-103">Update organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21a81-104">Mit dieser API können Sie die Eigenschaften der aktuell authentifizierten Organisation aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="21a81-104">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="21a81-105">In diesem Fall `organization` versteht man eine Auflistung von genau einen Datensatz, und so dessen **ID** in der Anforderung muss angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="21a81-105">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="21a81-106">Die **ID** wird auch als die **TenantId** der Organisation.</span><span class="sxs-lookup"><span data-stu-id="21a81-106">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="21a81-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="21a81-107">Permissions</span></span>

<span data-ttu-id="21a81-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21a81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21a81-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="21a81-110">Permission type</span></span> | <span data-ttu-id="21a81-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="21a81-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21a81-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="21a81-112">Delegated (work or school account)</span></span> | <span data-ttu-id="21a81-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="21a81-113">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="21a81-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="21a81-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21a81-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21a81-115">Not supported.</span></span> |
|<span data-ttu-id="21a81-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="21a81-116">Application</span></span> | <span data-ttu-id="21a81-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21a81-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="21a81-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="21a81-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="21a81-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="21a81-119">Request headers</span></span>

| <span data-ttu-id="21a81-120">Name</span><span class="sxs-lookup"><span data-stu-id="21a81-120">Name</span></span>       | <span data-ttu-id="21a81-121">Typ</span><span class="sxs-lookup"><span data-stu-id="21a81-121">Type</span></span> | <span data-ttu-id="21a81-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21a81-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="21a81-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21a81-123">Authorization</span></span>  | <span data-ttu-id="21a81-124">string</span><span class="sxs-lookup"><span data-stu-id="21a81-124">string</span></span>  | <span data-ttu-id="21a81-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="21a81-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21a81-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="21a81-127">Request body</span></span>

<span data-ttu-id="21a81-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="21a81-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="21a81-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="21a81-131">Property</span></span>     | <span data-ttu-id="21a81-132">Typ</span><span class="sxs-lookup"><span data-stu-id="21a81-132">Type</span></span>   |<span data-ttu-id="21a81-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21a81-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21a81-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="21a81-134">marketingNotificationEmails</span></span>|<span data-ttu-id="21a81-135">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="21a81-135">String collection</span></span>|                                        <span data-ttu-id="21a81-136">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="21a81-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="21a81-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="21a81-137">privacyProfile</span></span>|[<span data-ttu-id="21a81-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="21a81-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="21a81-139">Das Datenschutzprofil einer Organisation ( „statementUrl“ und „contactEmail“ festlegen).</span><span class="sxs-lookup"><span data-stu-id="21a81-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="21a81-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="21a81-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="21a81-141">String collection</span><span class="sxs-lookup"><span data-stu-id="21a81-141">String collection</span></span>||
|<span data-ttu-id="21a81-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="21a81-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="21a81-143">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="21a81-143">String collection</span></span>||
|<span data-ttu-id="21a81-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="21a81-144">technicalNotificationMails</span></span>|<span data-ttu-id="21a81-145">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="21a81-145">String collection</span></span>|                                        <span data-ttu-id="21a81-146">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="21a81-146">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="21a81-147">Da die Ressource **Organisation** [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `PATCH` Vorgang hinzufügen, aktualisieren und Löschen von Ihren eigenen app-spezifischen Daten in benutzerdefinierten Eigenschaften einer Erweiterung in einer vorhandenen Instanz der **Organisation** .</span><span class="sxs-lookup"><span data-stu-id="21a81-147">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="21a81-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="21a81-148">Response</span></span>

<span data-ttu-id="21a81-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="21a81-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21a81-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="21a81-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21a81-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="21a81-152">Request</span></span>
<span data-ttu-id="21a81-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="21a81-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{id}
Content-type: application/json
Content-length: 411

{
  "marketingNotificationEmails" : ["marketing@contoso.com"],
  "privacyProfile" :
    {
      "contactEmail":"alice@contoso.com",
      "statementUrl":"https://contoso.com/privacyStatement"
    },
  "securityComplianceNotificationMails" : ["security@contoso.com"],
  "securityComplianceNotificationPhones" : ["(123) 456-7890"],
  "technicalNotificationMails" : ["tech@contoso.com"]
}
```

##### <a name="response"></a><span data-ttu-id="21a81-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="21a81-154">Response</span></span>

<span data-ttu-id="21a81-155">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="21a81-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="21a81-156">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="21a81-156">See also</span></span>

- [<span data-ttu-id="21a81-157">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="21a81-157">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="21a81-158">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="21a81-158">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)

<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/organization-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
