---
title: Ressourcentyp oAuth2PermissionGrant
description: Stellt die OAuth 2.0-Bereiche (delegierten Berechtigungen) zu einer Anwendung (dargestellt durch ein Dienstprinzipal) erteilt wurden im Rahmen des Prozesses Zustimmung Benutzer oder Administrator an.
ms.openlocfilehash: 8fc5154ddba1b78976dc3e24c6712f9fc8944f43
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059346"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="a1905-103">Ressourcentyp oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a1905-103">oAuth2PermissionGrant resource type</span></span>

> <span data-ttu-id="a1905-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a1905-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1905-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a1905-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a1905-106">Stellt die OAuth 2.0-Bereiche (delegierten Berechtigungen) zu einer Anwendung (dargestellt durch ein Dienstprinzipal) erteilt wurden im Rahmen des Prozesses Zustimmung Benutzer oder Administrator an.</span><span class="sxs-lookup"><span data-stu-id="a1905-106">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1905-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a1905-107">JSON representation</span></span>

<span data-ttu-id="a1905-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a1905-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant"
}-->

```json
{
  "clientId": "string",
  "consentType": "string",
  "expiryTime": "String (timestamp)",
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string",
  "startTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="a1905-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a1905-109">Properties</span></span>
| <span data-ttu-id="a1905-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a1905-110">Property</span></span>     | <span data-ttu-id="a1905-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a1905-111">Type</span></span>   |<span data-ttu-id="a1905-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1905-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1905-113">clientId</span><span class="sxs-lookup"><span data-stu-id="a1905-113">clientId</span></span>|<span data-ttu-id="a1905-114">String</span><span class="sxs-lookup"><span data-stu-id="a1905-114">String</span></span>| <span data-ttu-id="a1905-115">Die Id des Prinzipals Dienst gewährt Ihr Einverständnis der Benutzer Identitätswechsel für den Zugriff auf die Ressource (dargestellt durch die ResourceId-Eigenschaft).</span><span class="sxs-lookup"><span data-stu-id="a1905-115">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="a1905-116">consentType</span><span class="sxs-lookup"><span data-stu-id="a1905-116">consentType</span></span>|<span data-ttu-id="a1905-117">String</span><span class="sxs-lookup"><span data-stu-id="a1905-117">String</span></span>| <span data-ttu-id="a1905-118">Gibt an, ob Zustimmung vom Administrator (im Namen der Organisation) oder von einer Person zur Verfügung gestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="a1905-118">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="a1905-119">Die möglichen Werte sind *AllPrincipals* oder *Prinzipal*.</span><span class="sxs-lookup"><span data-stu-id="a1905-119">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="a1905-120">expiryTime</span><span class="sxs-lookup"><span data-stu-id="a1905-120">expiryTime</span></span>|<span data-ttu-id="a1905-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1905-121">DateTimeOffset</span></span>| <span data-ttu-id="a1905-122">Derzeit ist der Ablauf Time-Wert ignoriert.</span><span class="sxs-lookup"><span data-stu-id="a1905-122">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="a1905-123">id</span><span class="sxs-lookup"><span data-stu-id="a1905-123">id</span></span>|<span data-ttu-id="a1905-124">String</span><span class="sxs-lookup"><span data-stu-id="a1905-124">String</span></span>| <span data-ttu-id="a1905-125">Eindeutiger Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="a1905-125">Unique identifier.</span></span> <span data-ttu-id="a1905-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a1905-126">Read-only.</span></span>|
|<span data-ttu-id="a1905-127">principalId</span><span class="sxs-lookup"><span data-stu-id="a1905-127">principalId</span></span>|<span data-ttu-id="a1905-128">String</span><span class="sxs-lookup"><span data-stu-id="a1905-128">String</span></span>| <span data-ttu-id="a1905-129">Wenn ConsentType *AllPrincipals* ist dieser Wert ist null, und die Zustimmung gilt für alle Benutzer in der Organisation.</span><span class="sxs-lookup"><span data-stu-id="a1905-129">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="a1905-130">Wenn ConsentType *Prinzipal*ist, gibt diese Eigenschaft die Id des Benutzers, der Zustimmung erteilt und gilt nur für diesen Benutzer an.</span><span class="sxs-lookup"><span data-stu-id="a1905-130">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="a1905-131">resourceId</span><span class="sxs-lookup"><span data-stu-id="a1905-131">resourceId</span></span>|<span data-ttu-id="a1905-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a1905-132">String</span></span>| <span data-ttu-id="a1905-133">Gibt die Id des Prinzipals Service Resource, der Zugriff gewährt wurde.</span><span class="sxs-lookup"><span data-stu-id="a1905-133">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="a1905-134">Bereich</span><span class="sxs-lookup"><span data-stu-id="a1905-134">scope</span></span>|<span data-ttu-id="a1905-135">String</span><span class="sxs-lookup"><span data-stu-id="a1905-135">String</span></span>| <span data-ttu-id="a1905-136">Gibt den Wert des Anspruchs [Bereich](/graph/permissions-reference) , der die Ressource Anwendung erwarten im Zugriffstoken OAuth 2.0 an.</span><span class="sxs-lookup"><span data-stu-id="a1905-136">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="a1905-137">Beispielsweise *User.Read*</span><span class="sxs-lookup"><span data-stu-id="a1905-137">For example, *User.Read*</span></span> |
|<span data-ttu-id="a1905-138">startTime</span><span class="sxs-lookup"><span data-stu-id="a1905-138">startTime</span></span>|<span data-ttu-id="a1905-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1905-139">DateTimeOffset</span></span>| <span data-ttu-id="a1905-140">Derzeit wird der Wert für die Startzeit ignoriert.</span><span class="sxs-lookup"><span data-stu-id="a1905-140">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a1905-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a1905-141">Relationships</span></span>
<span data-ttu-id="a1905-142">Keine</span><span class="sxs-lookup"><span data-stu-id="a1905-142">None</span></span>


## <a name="methods"></a><span data-ttu-id="a1905-143">Methoden</span><span class="sxs-lookup"><span data-stu-id="a1905-143">Methods</span></span>

| <span data-ttu-id="a1905-144">Methode</span><span class="sxs-lookup"><span data-stu-id="a1905-144">Method</span></span>           | <span data-ttu-id="a1905-145">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="a1905-145">Return Type</span></span>    |<span data-ttu-id="a1905-146">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1905-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a1905-147">Abrufen von oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a1905-147">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="a1905-148">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a1905-148">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="a1905-149">Lesen Sie Eigenschaften und Beziehungen des oAuth2PermissionGrant-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a1905-149">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="a1905-150">Liste oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="a1905-150">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="a1905-151">[oAuth2PermissionGrant](oauth2permissiongrant.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="a1905-151">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="a1905-152">Abrufen einer Liste von oauth2PermissionGrant-Objekten.</span><span class="sxs-lookup"><span data-stu-id="a1905-152">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="a1905-153">OAuth2PermissionGrant aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a1905-153">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="a1905-154">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a1905-154">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="a1905-155">OAuth2PermissionGrant-Objekt zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="a1905-155">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="a1905-156">OAuth2PermissionGrant löschen</span><span class="sxs-lookup"><span data-stu-id="a1905-156">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="a1905-157">Keines</span><span class="sxs-lookup"><span data-stu-id="a1905-157">None</span></span> |<span data-ttu-id="a1905-158">OAuth2PermissionGrant-Objekt zu löschen.</span><span class="sxs-lookup"><span data-stu-id="a1905-158">Delete oAuth2PermissionGrant object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->