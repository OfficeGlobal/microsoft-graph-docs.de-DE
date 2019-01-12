---
title: Administrativeunit aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AdministrativeUnit-Objekts.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cd82035e06fbd6135f4d2f6cbb7f6dfae9576f9a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932014"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="a0161-103">Administrativeunit aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a0161-103">Update administrativeunit</span></span>

> <span data-ttu-id="a0161-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a0161-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0161-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a0161-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a0161-106">Aktualisieren Sie die Eigenschaften eines [AdministrativeUnit](../resources/administrativeunit.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a0161-106">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a0161-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a0161-107">Permissions</span></span>
<span data-ttu-id="a0161-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0161-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a0161-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a0161-110">Permission type</span></span>      | <span data-ttu-id="a0161-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a0161-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0161-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a0161-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a0161-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a0161-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a0161-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a0161-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0161-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a0161-115">Not supported.</span></span>    |
|<span data-ttu-id="a0161-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a0161-116">Application</span></span> | <span data-ttu-id="a0161-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a0161-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0161-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0161-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a0161-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a0161-119">Request headers</span></span>

| <span data-ttu-id="a0161-120">Name</span><span class="sxs-lookup"><span data-stu-id="a0161-120">Name</span></span>      |<span data-ttu-id="a0161-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a0161-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a0161-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0161-122">Authorization</span></span>  | <span data-ttu-id="a0161-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a0161-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0161-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a0161-125">Request body</span></span>

<span data-ttu-id="a0161-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="a0161-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a0161-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a0161-129">Property</span></span>   | <span data-ttu-id="a0161-130">Typ</span><span class="sxs-lookup"><span data-stu-id="a0161-130">Type</span></span> |<span data-ttu-id="a0161-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a0161-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0161-132">description</span><span class="sxs-lookup"><span data-stu-id="a0161-132">description</span></span>|<span data-ttu-id="a0161-133">string</span><span class="sxs-lookup"><span data-stu-id="a0161-133">string</span></span>|<span data-ttu-id="a0161-134">Beschreibung für die administrative Einheit.</span><span class="sxs-lookup"><span data-stu-id="a0161-134">Description for the administrative unit.</span></span>|
|<span data-ttu-id="a0161-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a0161-135">displayName</span></span>|<span data-ttu-id="a0161-136">string</span><span class="sxs-lookup"><span data-stu-id="a0161-136">string</span></span>|<span data-ttu-id="a0161-137">Der Anzeigename für die administrative Einheit.</span><span class="sxs-lookup"><span data-stu-id="a0161-137">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="a0161-138">visibility</span><span class="sxs-lookup"><span data-stu-id="a0161-138">visibility</span></span>|<span data-ttu-id="a0161-139">string</span><span class="sxs-lookup"><span data-stu-id="a0161-139">string</span></span>|<span data-ttu-id="a0161-140">Sichtbarkeit für die administrative Einheit.</span><span class="sxs-lookup"><span data-stu-id="a0161-140">Visibility for the administrative unit.</span></span> <span data-ttu-id="a0161-141">Wenn dies nicht der Standardwert ist "public".</span><span class="sxs-lookup"><span data-stu-id="a0161-141">If not set then the default is "public".</span></span> <span data-ttu-id="a0161-142">Kann auf "HiddenMembership", der die Mitgliedschaft von nicht-Mitglieder verborgen festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="a0161-142">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="a0161-143">Da die Ressource **AdministrativeUnit** [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `PATCH` Vorgang hinzufügen, aktualisieren oder Löschen von Ihren eigenen app-spezifischen Daten in benutzerdefinierten Eigenschaften einer Erweiterung in einer vorhandenen **AdministrativeUnit** -Instanz.</span><span class="sxs-lookup"><span data-stu-id="a0161-143">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="a0161-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0161-144">Response</span></span>

<span data-ttu-id="a0161-145">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a0161-145">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a0161-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a0161-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a0161-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0161-147">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="a0161-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0161-148">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="a0161-149">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="a0161-149">See also</span></span>

- [<span data-ttu-id="a0161-150">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="a0161-150">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a0161-151">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="a0161-151">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update administrativeunit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
