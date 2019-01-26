---
title: Ressourcentyp oAuth2PermissionGrant
description: Stellt die OAuth 2.0-Bereiche (delegierten Berechtigungen) zu einer Anwendung (dargestellt durch ein Dienstprinzipal) erteilt wurden im Rahmen des Prozesses Zustimmung Benutzer oder Administrator an.
localization_priority: Normal
ms.openlocfilehash: 5d3d900395843f39645f61d1b984e3ed4f79d476
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576969"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="93e57-103">Ressourcentyp oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="93e57-103">oAuth2PermissionGrant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93e57-104">Stellt die OAuth 2.0-Bereiche (delegierten Berechtigungen) zu einer Anwendung (dargestellt durch ein Dienstprinzipal) erteilt wurden im Rahmen des Prozesses Zustimmung Benutzer oder Administrator an.</span><span class="sxs-lookup"><span data-stu-id="93e57-104">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="93e57-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="93e57-105">JSON representation</span></span>

<span data-ttu-id="93e57-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="93e57-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
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
## <a name="properties"></a><span data-ttu-id="93e57-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="93e57-107">Properties</span></span>
| <span data-ttu-id="93e57-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="93e57-108">Property</span></span>     | <span data-ttu-id="93e57-109">Typ</span><span class="sxs-lookup"><span data-stu-id="93e57-109">Type</span></span>   |<span data-ttu-id="93e57-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93e57-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93e57-111">clientId</span><span class="sxs-lookup"><span data-stu-id="93e57-111">clientId</span></span>|<span data-ttu-id="93e57-112">String</span><span class="sxs-lookup"><span data-stu-id="93e57-112">String</span></span>| <span data-ttu-id="93e57-113">Die Id des Prinzipals Dienst gewährt Ihr Einverständnis der Benutzer Identitätswechsel für den Zugriff auf die Ressource (dargestellt durch die ResourceId-Eigenschaft).</span><span class="sxs-lookup"><span data-stu-id="93e57-113">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="93e57-114">consentType</span><span class="sxs-lookup"><span data-stu-id="93e57-114">consentType</span></span>|<span data-ttu-id="93e57-115">String</span><span class="sxs-lookup"><span data-stu-id="93e57-115">String</span></span>| <span data-ttu-id="93e57-116">Gibt an, ob Zustimmung vom Administrator (im Namen der Organisation) oder von einer Person zur Verfügung gestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="93e57-116">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="93e57-117">Die möglichen Werte sind *AllPrincipals* oder *Prinzipal*.</span><span class="sxs-lookup"><span data-stu-id="93e57-117">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="93e57-118">expiryTime</span><span class="sxs-lookup"><span data-stu-id="93e57-118">expiryTime</span></span>|<span data-ttu-id="93e57-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93e57-119">DateTimeOffset</span></span>| <span data-ttu-id="93e57-120">Derzeit ist der Ablauf Time-Wert ignoriert.</span><span class="sxs-lookup"><span data-stu-id="93e57-120">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="93e57-121">id</span><span class="sxs-lookup"><span data-stu-id="93e57-121">id</span></span>|<span data-ttu-id="93e57-122">String</span><span class="sxs-lookup"><span data-stu-id="93e57-122">String</span></span>| <span data-ttu-id="93e57-123">Eindeutiger Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="93e57-123">Unique identifier.</span></span> <span data-ttu-id="93e57-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="93e57-124">Read-only.</span></span>|
|<span data-ttu-id="93e57-125">principalId</span><span class="sxs-lookup"><span data-stu-id="93e57-125">principalId</span></span>|<span data-ttu-id="93e57-126">String</span><span class="sxs-lookup"><span data-stu-id="93e57-126">String</span></span>| <span data-ttu-id="93e57-127">Wenn ConsentType *AllPrincipals* ist dieser Wert ist null, und die Zustimmung gilt für alle Benutzer in der Organisation.</span><span class="sxs-lookup"><span data-stu-id="93e57-127">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="93e57-128">Wenn ConsentType *Prinzipal*ist, gibt diese Eigenschaft die Id des Benutzers, der Zustimmung erteilt und gilt nur für diesen Benutzer an.</span><span class="sxs-lookup"><span data-stu-id="93e57-128">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="93e57-129">resourceId</span><span class="sxs-lookup"><span data-stu-id="93e57-129">resourceId</span></span>|<span data-ttu-id="93e57-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93e57-130">String</span></span>| <span data-ttu-id="93e57-131">Gibt die Id des Prinzipals Service Resource, der Zugriff gewährt wurde.</span><span class="sxs-lookup"><span data-stu-id="93e57-131">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="93e57-132">Bereich</span><span class="sxs-lookup"><span data-stu-id="93e57-132">scope</span></span>|<span data-ttu-id="93e57-133">String</span><span class="sxs-lookup"><span data-stu-id="93e57-133">String</span></span>| <span data-ttu-id="93e57-134">Gibt den Wert des Anspruchs [Bereich](/graph/permissions-reference) , der die Ressource Anwendung erwarten im Zugriffstoken OAuth 2.0 an.</span><span class="sxs-lookup"><span data-stu-id="93e57-134">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="93e57-135">Beispielsweise *User.Read*</span><span class="sxs-lookup"><span data-stu-id="93e57-135">For example, *User.Read*</span></span> |
|<span data-ttu-id="93e57-136">startTime</span><span class="sxs-lookup"><span data-stu-id="93e57-136">startTime</span></span>|<span data-ttu-id="93e57-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93e57-137">DateTimeOffset</span></span>| <span data-ttu-id="93e57-138">Derzeit wird der Wert für die Startzeit ignoriert.</span><span class="sxs-lookup"><span data-stu-id="93e57-138">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="93e57-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="93e57-139">Relationships</span></span>
<span data-ttu-id="93e57-140">Keine</span><span class="sxs-lookup"><span data-stu-id="93e57-140">None</span></span>


## <a name="methods"></a><span data-ttu-id="93e57-141">Methoden</span><span class="sxs-lookup"><span data-stu-id="93e57-141">Methods</span></span>

| <span data-ttu-id="93e57-142">Methode</span><span class="sxs-lookup"><span data-stu-id="93e57-142">Method</span></span>           | <span data-ttu-id="93e57-143">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="93e57-143">Return Type</span></span>    |<span data-ttu-id="93e57-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93e57-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="93e57-145">Abrufen von oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="93e57-145">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="93e57-146">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="93e57-146">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="93e57-147">Lesen Sie Eigenschaften und Beziehungen des oAuth2PermissionGrant-Objekts.</span><span class="sxs-lookup"><span data-stu-id="93e57-147">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="93e57-148">Liste oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="93e57-148">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="93e57-149">[oAuth2PermissionGrant](oauth2permissiongrant.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="93e57-149">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="93e57-150">Abrufen einer Liste von oauth2PermissionGrant-Objekten.</span><span class="sxs-lookup"><span data-stu-id="93e57-150">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="93e57-151">OAuth2PermissionGrant aktualisieren</span><span class="sxs-lookup"><span data-stu-id="93e57-151">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="93e57-152">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="93e57-152">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="93e57-153">OAuth2PermissionGrant-Objekt zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="93e57-153">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="93e57-154">OAuth2PermissionGrant löschen</span><span class="sxs-lookup"><span data-stu-id="93e57-154">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="93e57-155">Keine</span><span class="sxs-lookup"><span data-stu-id="93e57-155">None</span></span> |<span data-ttu-id="93e57-156">OAuth2PermissionGrant-Objekt zu löschen.</span><span class="sxs-lookup"><span data-stu-id="93e57-156">Delete oAuth2PermissionGrant object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/oauth2permissiongrant.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
