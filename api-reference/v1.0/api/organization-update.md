---
title: Organisation aktualisieren
description: Mit dieser API können Sie die Eigenschaften der aktuell authentifizierten Organisation aktualisieren.
localization_priority: Normal
ms.openlocfilehash: 83b1514831e930e3eabe6e6a78203c44ec3b5b3c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834958"
---
# <a name="update-organization"></a><span data-ttu-id="cb142-103">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="cb142-103">Update organization</span></span>

<span data-ttu-id="cb142-104">Mit dieser API können Sie die Eigenschaften der aktuell authentifizierten Organisation aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="cb142-104">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="cb142-105">In diesem Fall `organization` versteht man eine Auflistung von genau einen Datensatz, und so dessen **ID** in der Anforderung muss angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="cb142-105">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="cb142-106">Die **ID** wird auch als die **TenantId** der Organisation.</span><span class="sxs-lookup"><span data-stu-id="cb142-106">The **ID** is also known as the **tenantId** of the organization.</span></span>


## <a name="permissions"></a><span data-ttu-id="cb142-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cb142-107">Permissions</span></span>

<span data-ttu-id="cb142-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb142-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb142-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cb142-110">Permission type</span></span> | <span data-ttu-id="cb142-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cb142-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb142-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cb142-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cb142-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cb142-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cb142-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cb142-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb142-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cb142-115">Not supported.</span></span>    |
|<span data-ttu-id="cb142-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cb142-116">Application</span></span> | <span data-ttu-id="cb142-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cb142-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb142-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb142-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}

```

## <a name="request-headers"></a><span data-ttu-id="cb142-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cb142-119">Request headers</span></span>

| <span data-ttu-id="cb142-120">Name</span><span class="sxs-lookup"><span data-stu-id="cb142-120">Name</span></span>       | <span data-ttu-id="cb142-121">Typ</span><span class="sxs-lookup"><span data-stu-id="cb142-121">Type</span></span> | <span data-ttu-id="cb142-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb142-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cb142-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb142-123">Authorization</span></span>  | <span data-ttu-id="cb142-124">string</span><span class="sxs-lookup"><span data-stu-id="cb142-124">string</span></span>  | <span data-ttu-id="cb142-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cb142-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb142-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cb142-127">Request body</span></span>

<span data-ttu-id="cb142-128">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="cb142-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="cb142-129">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="cb142-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="cb142-130">Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="cb142-130">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cb142-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cb142-131">Property</span></span>     | <span data-ttu-id="cb142-132">Typ</span><span class="sxs-lookup"><span data-stu-id="cb142-132">Type</span></span>   |<span data-ttu-id="cb142-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb142-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb142-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="cb142-134">marketingNotificationEmails</span></span>|<span data-ttu-id="cb142-135">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="cb142-135">String collection</span></span>|                                        <span data-ttu-id="cb142-136">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="cb142-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="cb142-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="cb142-137">privacyProfile</span></span>|[<span data-ttu-id="cb142-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="cb142-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="cb142-139">Das Datenschutzprofil einer Organisation ( „statementUrl“ und „contactEmail“ festlegen).</span><span class="sxs-lookup"><span data-stu-id="cb142-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="cb142-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="cb142-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="cb142-141">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="cb142-141">String collection</span></span>||
|<span data-ttu-id="cb142-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="cb142-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="cb142-143">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="cb142-143">String collection</span></span>||
|<span data-ttu-id="cb142-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="cb142-144">technicalNotificationMails</span></span>|<span data-ttu-id="cb142-145">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="cb142-145">String collection</span></span>|                                        <span data-ttu-id="cb142-146">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="cb142-146">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="cb142-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb142-147">Response</span></span>

<span data-ttu-id="cb142-148">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cb142-148">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cb142-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cb142-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb142-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb142-150">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/{id}
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

### <a name="response"></a><span data-ttu-id="cb142-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb142-151">Response</span></span>

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
