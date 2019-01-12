---
title: Aktualisieren von groupLifecyclePolicy
description: Aktualisieren Sie die Eigenschaften eines groupLifecyclePolicygroupLifecyclePolicy-Ressourcentyp-Objekts.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 5914f0047a591ba53b160ba988342c13f0741fd6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955961"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="2b8a3-103">Aktualisieren von groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="2b8a3-103">Update groupLifecyclePolicy</span></span>

> <span data-ttu-id="2b8a3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2b8a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b8a3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2b8a3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b8a3-106">Aktualisieren Sie die Eigenschaften eines groupLifecyclePolicy[groupLifecyclePolicy-Ressourcentyp](../resources/grouplifecyclepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2b8a3-106">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b8a3-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2b8a3-107">Permissions</span></span>

<span data-ttu-id="2b8a3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b8a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="2b8a3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2b8a3-110">Permission type</span></span>      | <span data-ttu-id="2b8a3-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2b8a3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b8a3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2b8a3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2b8a3-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b8a3-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="2b8a3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2b8a3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b8a3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b8a3-115">Not supported</span></span> |
|<span data-ttu-id="2b8a3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2b8a3-116">Application</span></span> | <span data-ttu-id="2b8a3-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b8a3-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b8a3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b8a3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="2b8a3-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2b8a3-119">Optional request headers</span></span>
| <span data-ttu-id="2b8a3-120">Name</span><span class="sxs-lookup"><span data-stu-id="2b8a3-120">Name</span></span> | <span data-ttu-id="2b8a3-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b8a3-121">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="2b8a3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b8a3-122">Authorization</span></span> | <span data-ttu-id="2b8a3-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2b8a3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2b8a3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2b8a3-125">Content-Type</span></span>  | <span data-ttu-id="2b8a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b8a3-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2b8a3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2b8a3-127">Request body</span></span>

<span data-ttu-id="2b8a3-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="2b8a3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2b8a3-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2b8a3-131">Property</span></span> | <span data-ttu-id="2b8a3-132">Typ</span><span class="sxs-lookup"><span data-stu-id="2b8a3-132">Type</span></span> | <span data-ttu-id="2b8a3-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b8a3-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2b8a3-134">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="2b8a3-134">alternateNotificationEmails</span></span>|<span data-ttu-id="2b8a3-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2b8a3-135">String</span></span>| <span data-ttu-id="2b8a3-136">Liste der E-Mail-Adressen, an die Benachrichtigungen für Gruppen ohne Besitzer gesendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="2b8a3-136">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="2b8a3-137">Mehrere E-Mail-Adressen können durch ein Semikolon voneinander getrennt definiert werden.</span><span class="sxs-lookup"><span data-stu-id="2b8a3-137">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="2b8a3-138">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="2b8a3-138">groupLifetimeInDays</span></span>|<span data-ttu-id="2b8a3-139">Int32</span><span class="sxs-lookup"><span data-stu-id="2b8a3-139">Int32</span></span>| <span data-ttu-id="2b8a3-140">Anzahl von Tagen, bis eine Gruppe abläuft und verlängert werden muss.</span><span class="sxs-lookup"><span data-stu-id="2b8a3-140">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="2b8a3-141">Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der definierten Tage verlängert.</span><span class="sxs-lookup"><span data-stu-id="2b8a3-141">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="2b8a3-142">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="2b8a3-142">managedGroupTypes</span></span>|<span data-ttu-id="2b8a3-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2b8a3-143">String</span></span>| <span data-ttu-id="2b8a3-144">Der Gruppentyp, für den die Ablaufrichtlinie gilt.</span><span class="sxs-lookup"><span data-stu-id="2b8a3-144">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="2b8a3-145">Mögliche Werte sind **Alle**, **Ausgewählte** oder **Keine**.</span><span class="sxs-lookup"><span data-stu-id="2b8a3-145">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="2b8a3-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b8a3-146">Response</span></span>

<span data-ttu-id="2b8a3-147">Wenn erfolgreich ausgeführt, gibt diese Methode den Antwortcode `200 OK` und ein aktualisiertes [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2b8a3-147">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b8a3-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2b8a3-148">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2b8a3-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b8a3-149">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_grouplifecyclepolicy"
}-->
```http
PATCH https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
Content-type: application/json
Content-length: 151

{
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="2b8a3-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b8a3-150">Response</span></span>
<span data-ttu-id="2b8a3-151">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="2b8a3-151">Note: The response object shown here may be truncated for brevity.</span></span> 
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
