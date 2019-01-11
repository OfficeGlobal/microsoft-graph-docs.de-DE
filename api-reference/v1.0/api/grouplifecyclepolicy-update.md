---
title: Aktualisieren von groupLifecyclePolicy
description: Aktualisieren Sie die Eigenschaften eines groupLifecyclePolicygroupLifecyclePolicy-Ressourcentyp-Objekts.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 66b0d19ac4f1ae24ec76702ffb55542b363e43ab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864869"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="3c074-103">Aktualisieren von groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="3c074-103">Update groupLifecyclePolicy</span></span>

<span data-ttu-id="3c074-104">Aktualisieren Sie die Eigenschaften eines groupLifecyclePolicy[groupLifecyclePolicy-Ressourcentyp](../resources/grouplifecyclepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3c074-104">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c074-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3c074-105">Permissions</span></span>

<span data-ttu-id="3c074-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c074-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 
|<span data-ttu-id="3c074-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3c074-108">Permission type</span></span>      | <span data-ttu-id="3c074-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3c074-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c074-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3c074-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3c074-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c074-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="3c074-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3c074-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c074-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3c074-113">Not supported.</span></span>    |
|<span data-ttu-id="3c074-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3c074-114">Application</span></span> | <span data-ttu-id="3c074-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c074-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c074-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3c074-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="3c074-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3c074-117">Optional request headers</span></span>
| <span data-ttu-id="3c074-118">Name</span><span class="sxs-lookup"><span data-stu-id="3c074-118">Name</span></span> | <span data-ttu-id="3c074-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c074-119">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="3c074-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c074-120">Authorization</span></span> | <span data-ttu-id="3c074-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3c074-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3c074-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3c074-123">Content-Type</span></span>  | <span data-ttu-id="3c074-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3c074-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3c074-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3c074-125">Request body</span></span>

<span data-ttu-id="3c074-126">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="3c074-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3c074-127">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="3c074-127">Existing properties that are not included in the request body maintain their previous values or are recalculated based on changes to other property values.</span></span> <span data-ttu-id="3c074-128">Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="3c074-128">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3c074-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3c074-129">Property</span></span> | <span data-ttu-id="3c074-130">Typ</span><span class="sxs-lookup"><span data-stu-id="3c074-130">Type</span></span> | <span data-ttu-id="3c074-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c074-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3c074-132">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="3c074-132">alternateNotificationEmails</span></span>|<span data-ttu-id="3c074-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3c074-133">String</span></span>| <span data-ttu-id="3c074-134">Liste der E-Mail-Adressen, an die Benachrichtigungen für Gruppen ohne Besitzer gesendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="3c074-134">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="3c074-135">Mehrere E-Mail-Adressen können durch ein Semikolon voneinander getrennt definiert werden.</span><span class="sxs-lookup"><span data-stu-id="3c074-135">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="3c074-136">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="3c074-136">groupLifetimeInDays</span></span>|<span data-ttu-id="3c074-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3c074-137">Int32</span></span>| <span data-ttu-id="3c074-138">Anzahl von Tagen, bis eine Gruppe abläuft und verlängert werden muss.</span><span class="sxs-lookup"><span data-stu-id="3c074-138">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="3c074-139">Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der definierten Tage verlängert.</span><span class="sxs-lookup"><span data-stu-id="3c074-139">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="3c074-140">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="3c074-140">managedGroupTypes</span></span>|<span data-ttu-id="3c074-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3c074-141">String</span></span>| <span data-ttu-id="3c074-142">Der Gruppentyp, für den die Ablaufrichtlinie gilt.</span><span class="sxs-lookup"><span data-stu-id="3c074-142">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="3c074-143">Mögliche Werte sind **Alle**, **Ausgewählte** oder **Keine**.</span><span class="sxs-lookup"><span data-stu-id="3c074-143">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="3c074-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="3c074-144">Response</span></span>

<span data-ttu-id="3c074-145">Wenn erfolgreich ausgeführt, gibt diese Methode den Antwortcode `200 OK` und ein aktualisiertes [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3c074-145">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3c074-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3c074-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3c074-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3c074-147">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_grouplifecyclepolicy"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="3c074-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="3c074-148">Response</span></span>
<span data-ttu-id="3c074-149">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="3c074-149">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "id": "id-value",
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
