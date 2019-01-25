---
title: Administrativeunit aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AdministrativeUnit-Objekts.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f3c57f8784bf642df7944bc6295ebd4fadc0ba43
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511156"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="393ed-103">Administrativeunit aktualisieren</span><span class="sxs-lookup"><span data-stu-id="393ed-103">Update administrativeunit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="393ed-104">Aktualisieren Sie die Eigenschaften eines [AdministrativeUnit](../resources/administrativeunit.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="393ed-104">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="393ed-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="393ed-105">Permissions</span></span>
<span data-ttu-id="393ed-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="393ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="393ed-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="393ed-108">Permission type</span></span>      | <span data-ttu-id="393ed-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="393ed-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="393ed-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="393ed-110">Delegated (work or school account)</span></span> | <span data-ttu-id="393ed-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="393ed-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="393ed-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="393ed-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="393ed-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="393ed-113">Not supported.</span></span>    |
|<span data-ttu-id="393ed-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="393ed-114">Application</span></span> | <span data-ttu-id="393ed-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="393ed-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="393ed-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="393ed-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="393ed-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="393ed-117">Request headers</span></span>

| <span data-ttu-id="393ed-118">Name</span><span class="sxs-lookup"><span data-stu-id="393ed-118">Name</span></span>      |<span data-ttu-id="393ed-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="393ed-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="393ed-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="393ed-120">Authorization</span></span>  | <span data-ttu-id="393ed-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="393ed-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="393ed-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="393ed-123">Request body</span></span>

<span data-ttu-id="393ed-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="393ed-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="393ed-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="393ed-127">Property</span></span>   | <span data-ttu-id="393ed-128">Typ</span><span class="sxs-lookup"><span data-stu-id="393ed-128">Type</span></span> |<span data-ttu-id="393ed-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="393ed-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="393ed-130">description</span><span class="sxs-lookup"><span data-stu-id="393ed-130">description</span></span>|<span data-ttu-id="393ed-131">string</span><span class="sxs-lookup"><span data-stu-id="393ed-131">string</span></span>|<span data-ttu-id="393ed-132">Beschreibung für die administrative Einheit.</span><span class="sxs-lookup"><span data-stu-id="393ed-132">Description for the administrative unit.</span></span>|
|<span data-ttu-id="393ed-133">displayName</span><span class="sxs-lookup"><span data-stu-id="393ed-133">displayName</span></span>|<span data-ttu-id="393ed-134">string</span><span class="sxs-lookup"><span data-stu-id="393ed-134">string</span></span>|<span data-ttu-id="393ed-135">Der Anzeigename für die administrative Einheit.</span><span class="sxs-lookup"><span data-stu-id="393ed-135">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="393ed-136">visibility</span><span class="sxs-lookup"><span data-stu-id="393ed-136">visibility</span></span>|<span data-ttu-id="393ed-137">string</span><span class="sxs-lookup"><span data-stu-id="393ed-137">string</span></span>|<span data-ttu-id="393ed-138">Sichtbarkeit für die administrative Einheit.</span><span class="sxs-lookup"><span data-stu-id="393ed-138">Visibility for the administrative unit.</span></span> <span data-ttu-id="393ed-139">Wenn dies nicht der Standardwert ist "public".</span><span class="sxs-lookup"><span data-stu-id="393ed-139">If not set then the default is "public".</span></span> <span data-ttu-id="393ed-140">Kann auf "HiddenMembership", der die Mitgliedschaft von nicht-Mitglieder verborgen festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="393ed-140">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="393ed-141">Da die Ressource **AdministrativeUnit** [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `PATCH` Vorgang hinzufügen, aktualisieren oder Löschen von Ihren eigenen app-spezifischen Daten in benutzerdefinierten Eigenschaften einer Erweiterung in einer vorhandenen **AdministrativeUnit** -Instanz.</span><span class="sxs-lookup"><span data-stu-id="393ed-141">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="393ed-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="393ed-142">Response</span></span>

<span data-ttu-id="393ed-143">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="393ed-143">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="393ed-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="393ed-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="393ed-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="393ed-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_administrativeunit"
}-->
```http
PATCH https://graph.microsoft.com/beta/administrativeUnits/{id}
Content-type: application/json
Content-length: 114

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value"
}
```

##### <a name="response"></a><span data-ttu-id="393ed-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="393ed-146">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="393ed-147">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="393ed-147">See also</span></span>

- [<span data-ttu-id="393ed-148">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="393ed-148">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="393ed-149">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="393ed-149">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update administrativeunit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
