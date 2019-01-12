---
title: Organisation aktualisieren
description: Mit dieser API können Sie die Eigenschaften der aktuell authentifizierten Organisation aktualisieren.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5ed49dcd0546fedf16572bcf75a8c4366395f1fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964438"
---
# <a name="update-organization"></a><span data-ttu-id="509d9-103">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="509d9-103">Update organization</span></span>

> <span data-ttu-id="509d9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="509d9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="509d9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="509d9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="509d9-106">Mit dieser API können Sie die Eigenschaften der aktuell authentifizierten Organisation aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="509d9-106">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="509d9-107">In diesem Fall `organization` versteht man eine Auflistung von genau einen Datensatz, und so dessen **ID** in der Anforderung muss angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="509d9-107">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="509d9-108">Die **ID** wird auch als die **TenantId** der Organisation.</span><span class="sxs-lookup"><span data-stu-id="509d9-108">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="509d9-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="509d9-109">Permissions</span></span>

<span data-ttu-id="509d9-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="509d9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="509d9-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="509d9-112">Permission type</span></span> | <span data-ttu-id="509d9-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="509d9-113">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="509d9-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="509d9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="509d9-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="509d9-115">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="509d9-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="509d9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="509d9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="509d9-117">Not supported.</span></span> |
|<span data-ttu-id="509d9-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="509d9-118">Application</span></span> | <span data-ttu-id="509d9-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="509d9-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="509d9-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="509d9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="509d9-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="509d9-121">Request headers</span></span>

| <span data-ttu-id="509d9-122">Name</span><span class="sxs-lookup"><span data-stu-id="509d9-122">Name</span></span>       | <span data-ttu-id="509d9-123">Typ</span><span class="sxs-lookup"><span data-stu-id="509d9-123">Type</span></span> | <span data-ttu-id="509d9-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="509d9-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="509d9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="509d9-125">Authorization</span></span>  | <span data-ttu-id="509d9-126">string</span><span class="sxs-lookup"><span data-stu-id="509d9-126">string</span></span>  | <span data-ttu-id="509d9-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="509d9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="509d9-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="509d9-129">Request body</span></span>

<span data-ttu-id="509d9-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="509d9-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="509d9-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="509d9-133">Property</span></span>     | <span data-ttu-id="509d9-134">Typ</span><span class="sxs-lookup"><span data-stu-id="509d9-134">Type</span></span>   |<span data-ttu-id="509d9-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="509d9-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="509d9-136">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="509d9-136">marketingNotificationEmails</span></span>|<span data-ttu-id="509d9-137">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="509d9-137">String collection</span></span>|                                        <span data-ttu-id="509d9-138">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="509d9-138">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="509d9-139">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="509d9-139">privacyProfile</span></span>|[<span data-ttu-id="509d9-140">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="509d9-140">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="509d9-141">Das Datenschutzprofil einer Organisation ( „statementUrl“ und „contactEmail“ festlegen).</span><span class="sxs-lookup"><span data-stu-id="509d9-141">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="509d9-142">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="509d9-142">securityComplianceNotificationMails</span></span>|<span data-ttu-id="509d9-143">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="509d9-143">String collection</span></span>||
|<span data-ttu-id="509d9-144">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="509d9-144">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="509d9-145">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="509d9-145">String collection</span></span>||
|<span data-ttu-id="509d9-146">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="509d9-146">technicalNotificationMails</span></span>|<span data-ttu-id="509d9-147">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="509d9-147">String collection</span></span>|                                        <span data-ttu-id="509d9-148">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="509d9-148">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="509d9-149">Da die Ressource **Organisation** [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `PATCH` Vorgang hinzufügen, aktualisieren und Löschen von Ihren eigenen app-spezifischen Daten in benutzerdefinierten Eigenschaften einer Erweiterung in einer vorhandenen Instanz der **Organisation** .</span><span class="sxs-lookup"><span data-stu-id="509d9-149">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="509d9-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="509d9-150">Response</span></span>

<span data-ttu-id="509d9-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="509d9-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="509d9-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="509d9-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="509d9-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="509d9-154">Request</span></span>
<span data-ttu-id="509d9-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="509d9-155">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="509d9-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="509d9-156">Response</span></span>

<span data-ttu-id="509d9-157">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="509d9-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="509d9-158">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="509d9-158">See also</span></span>

- [<span data-ttu-id="509d9-159">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="509d9-159">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="509d9-160">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="509d9-160">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)

<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
