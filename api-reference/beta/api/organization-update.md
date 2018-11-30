---
title: Organisation aktualisieren
description: Mit dieser API können Sie die Eigenschaften der aktuell authentifizierten Organisation aktualisieren.
ms.openlocfilehash: 62e03d7bee58f14acc5d5ace12d55f95d1d07a2d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060009"
---
# <a name="update-organization"></a><span data-ttu-id="2a97e-103">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2a97e-103">Update organization</span></span>

> <span data-ttu-id="2a97e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2a97e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a97e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a97e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2a97e-106">Mit dieser API können Sie die Eigenschaften der aktuell authentifizierten Organisation aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="2a97e-106">Update the properties of the currently authenticated organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="2a97e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2a97e-107">Permissions</span></span>
<span data-ttu-id="2a97e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a97e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a97e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2a97e-110">Permission type</span></span> | <span data-ttu-id="2a97e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2a97e-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a97e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2a97e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2a97e-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2a97e-113">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="2a97e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2a97e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a97e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a97e-115">Not supported.</span></span> |
|<span data-ttu-id="2a97e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2a97e-116">Application</span></span> | <span data-ttu-id="2a97e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a97e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a97e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a97e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /organization

```
## <a name="request-headers"></a><span data-ttu-id="2a97e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2a97e-119">Request headers</span></span>
| <span data-ttu-id="2a97e-120">Name</span><span class="sxs-lookup"><span data-stu-id="2a97e-120">Name</span></span>       | <span data-ttu-id="2a97e-121">Typ</span><span class="sxs-lookup"><span data-stu-id="2a97e-121">Type</span></span> | <span data-ttu-id="2a97e-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a97e-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2a97e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a97e-123">Authorization</span></span>  | <span data-ttu-id="2a97e-124">string</span><span class="sxs-lookup"><span data-stu-id="2a97e-124">string</span></span>  | <span data-ttu-id="2a97e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2a97e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a97e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2a97e-127">Request body</span></span>
<span data-ttu-id="2a97e-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="2a97e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2a97e-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a97e-131">Property</span></span>     | <span data-ttu-id="2a97e-132">Typ</span><span class="sxs-lookup"><span data-stu-id="2a97e-132">Type</span></span>   |<span data-ttu-id="2a97e-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a97e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a97e-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="2a97e-134">marketingNotificationEmails</span></span>|<span data-ttu-id="2a97e-135">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="2a97e-135">String collection</span></span>|                                        <span data-ttu-id="2a97e-136">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="2a97e-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="2a97e-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="2a97e-137">privacyProfile</span></span>|[<span data-ttu-id="2a97e-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="2a97e-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="2a97e-139">Das Datenschutzprofil einer Organisation ( „statementUrl“ und „contactEmail“ festlegen).</span><span class="sxs-lookup"><span data-stu-id="2a97e-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="2a97e-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="2a97e-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="2a97e-141">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="2a97e-141">String collection</span></span>||
|<span data-ttu-id="2a97e-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="2a97e-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="2a97e-143">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="2a97e-143">String collection</span></span>||
|<span data-ttu-id="2a97e-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="2a97e-144">technicalNotificationMails</span></span>|<span data-ttu-id="2a97e-145">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="2a97e-145">String collection</span></span>|                                        <span data-ttu-id="2a97e-146">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="2a97e-146">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="2a97e-147">Da die Ressource **Organisation** [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `PATCH` Vorgang hinzufügen, aktualisieren und Löschen von Ihren eigenen app-spezifischen Daten in benutzerdefinierten Eigenschaften einer Erweiterung in einer vorhandenen Instanz der **Organisation** .</span><span class="sxs-lookup"><span data-stu-id="2a97e-147">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="2a97e-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a97e-148">Response</span></span>

<span data-ttu-id="2a97e-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a97e-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a97e-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2a97e-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a97e-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a97e-152">Request</span></span>
<span data-ttu-id="2a97e-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2a97e-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->
```http
PATCH https://graph.microsoft.com/beta/organization
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
##### <a name="response"></a><span data-ttu-id="2a97e-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a97e-154">Response</span></span>
<span data-ttu-id="2a97e-155">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2a97e-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="2a97e-156">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="2a97e-156">See also</span></span>

- [<span data-ttu-id="2a97e-157">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="2a97e-157">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="2a97e-158">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="2a97e-158">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
