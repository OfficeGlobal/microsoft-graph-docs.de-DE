---
title: Organisation aktualisieren
description: Mit dieser API können Sie die Eigenschaften der aktuell authentifizierten Organisation aktualisieren.
ms.openlocfilehash: ac07f3ded31f8d6c7169d24208ed7e8cf967e07a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019193"
---
# <a name="update-organization"></a><span data-ttu-id="adcc4-103">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="adcc4-103">Update organization</span></span>

<span data-ttu-id="adcc4-104">Mit dieser API können Sie die Eigenschaften der aktuell authentifizierten Organisation aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="adcc4-104">Update the properties of the currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="adcc4-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="adcc4-105">Permissions</span></span>

<span data-ttu-id="adcc4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adcc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adcc4-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="adcc4-108">Permission type</span></span> | <span data-ttu-id="adcc4-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="adcc4-109">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="adcc4-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="adcc4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="adcc4-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="adcc4-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="adcc4-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="adcc4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adcc4-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="adcc4-113">Not supported.</span></span>    |
|<span data-ttu-id="adcc4-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="adcc4-114">Application</span></span> | <span data-ttu-id="adcc4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="adcc4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="adcc4-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="adcc4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization

```

## <a name="request-headers"></a><span data-ttu-id="adcc4-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="adcc4-117">Request headers</span></span>

| <span data-ttu-id="adcc4-118">Name</span><span class="sxs-lookup"><span data-stu-id="adcc4-118">Name</span></span>       | <span data-ttu-id="adcc4-119">Typ</span><span class="sxs-lookup"><span data-stu-id="adcc4-119">Type</span></span> | <span data-ttu-id="adcc4-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="adcc4-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="adcc4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="adcc4-121">Authorization</span></span>  | <span data-ttu-id="adcc4-122">string</span><span class="sxs-lookup"><span data-stu-id="adcc4-122">string</span></span>  | <span data-ttu-id="adcc4-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="adcc4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="adcc4-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="adcc4-125">Request body</span></span>
<span data-ttu-id="adcc4-126">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="adcc4-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="adcc4-127">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="adcc4-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="adcc4-128">Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="adcc4-128">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="adcc4-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="adcc4-129">Property</span></span>     | <span data-ttu-id="adcc4-130">Typ</span><span class="sxs-lookup"><span data-stu-id="adcc4-130">Type</span></span>   |<span data-ttu-id="adcc4-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="adcc4-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="adcc4-132">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="adcc4-132">marketingNotificationEmails</span></span>|<span data-ttu-id="adcc4-133">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="adcc4-133">String collection</span></span>|                                        <span data-ttu-id="adcc4-134">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="adcc4-134">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="adcc4-135">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="adcc4-135">privacyProfile</span></span>|[<span data-ttu-id="adcc4-136">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="adcc4-136">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="adcc4-137">Das Datenschutzprofil einer Organisation ( „statementUrl“ und „contactEmail“ festlegen).</span><span class="sxs-lookup"><span data-stu-id="adcc4-137">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="adcc4-138">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="adcc4-138">securityComplianceNotificationMails</span></span>|<span data-ttu-id="adcc4-139">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="adcc4-139">String collection</span></span>||
|<span data-ttu-id="adcc4-140">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="adcc4-140">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="adcc4-141">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="adcc4-141">String collection</span></span>||
|<span data-ttu-id="adcc4-142">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="adcc4-142">technicalNotificationMails</span></span>|<span data-ttu-id="adcc4-143">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="adcc4-143">String collection</span></span>|                                        <span data-ttu-id="adcc4-144">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="adcc4-144">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="adcc4-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="adcc4-145">Response</span></span>

<span data-ttu-id="adcc4-146">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="adcc4-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="adcc4-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="adcc4-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="adcc4-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="adcc4-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization
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

### <a name="response"></a><span data-ttu-id="adcc4-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="adcc4-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
