---
title: Ressourcentyp oAuth2PermissionGrant
description: Stellt die OAuth 2.0-Bereiche (delegierten Berechtigungen) zu einer Anwendung (dargestellt durch ein Dienstprinzipal) erteilt wurden im Rahmen des Prozesses Zustimmung Benutzer oder Administrator an.
localization_priority: Normal
ms.openlocfilehash: ea6486aedca4c3fcf73e59a5652ccf517fb01ddc
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640777"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="f0e38-103">Ressourcentyp oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="f0e38-103">oAuth2PermissionGrant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0e38-104">Stellt die OAuth 2.0-Bereiche (delegierten Berechtigungen) zu einer Anwendung (dargestellt durch ein Dienstprinzipal) erteilt wurden im Rahmen des Prozesses Zustimmung Benutzer oder Administrator an.</span><span class="sxs-lookup"><span data-stu-id="f0e38-104">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0e38-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f0e38-105">JSON representation</span></span>

<span data-ttu-id="f0e38-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f0e38-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="f0e38-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f0e38-107">Properties</span></span>
| <span data-ttu-id="f0e38-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f0e38-108">Property</span></span>     | <span data-ttu-id="f0e38-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f0e38-109">Type</span></span>   |<span data-ttu-id="f0e38-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0e38-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0e38-111">clientId</span><span class="sxs-lookup"><span data-stu-id="f0e38-111">clientId</span></span>|<span data-ttu-id="f0e38-112">String</span><span class="sxs-lookup"><span data-stu-id="f0e38-112">String</span></span>| <span data-ttu-id="f0e38-113">Die Id des Prinzipals Dienst gewährt Ihr Einverständnis der Benutzer Identitätswechsel für den Zugriff auf die Ressource (dargestellt durch die ResourceId-Eigenschaft).</span><span class="sxs-lookup"><span data-stu-id="f0e38-113">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="f0e38-114">consentType</span><span class="sxs-lookup"><span data-stu-id="f0e38-114">consentType</span></span>|<span data-ttu-id="f0e38-115">String</span><span class="sxs-lookup"><span data-stu-id="f0e38-115">String</span></span>| <span data-ttu-id="f0e38-116">Gibt an, ob Zustimmung vom Administrator (im Namen der Organisation) oder von einer Person zur Verfügung gestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="f0e38-116">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="f0e38-117">Die möglichen Werte sind *AllPrincipals* oder *Prinzipal*.</span><span class="sxs-lookup"><span data-stu-id="f0e38-117">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="f0e38-118">expiryTime</span><span class="sxs-lookup"><span data-stu-id="f0e38-118">expiryTime</span></span>|<span data-ttu-id="f0e38-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0e38-119">DateTimeOffset</span></span>| <span data-ttu-id="f0e38-120">Derzeit ist der Ablauf Time-Wert ignoriert.</span><span class="sxs-lookup"><span data-stu-id="f0e38-120">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="f0e38-121">id</span><span class="sxs-lookup"><span data-stu-id="f0e38-121">id</span></span>|<span data-ttu-id="f0e38-122">String</span><span class="sxs-lookup"><span data-stu-id="f0e38-122">String</span></span>| <span data-ttu-id="f0e38-123">Eindeutiger Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="f0e38-123">Unique identifier.</span></span> <span data-ttu-id="f0e38-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f0e38-124">Read-only.</span></span>|
|<span data-ttu-id="f0e38-125">principalId</span><span class="sxs-lookup"><span data-stu-id="f0e38-125">principalId</span></span>|<span data-ttu-id="f0e38-126">String</span><span class="sxs-lookup"><span data-stu-id="f0e38-126">String</span></span>| <span data-ttu-id="f0e38-127">Wenn ConsentType *AllPrincipals* ist dieser Wert ist null, und die Zustimmung gilt für alle Benutzer in der Organisation.</span><span class="sxs-lookup"><span data-stu-id="f0e38-127">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="f0e38-128">Wenn ConsentType *Prinzipal*ist, gibt diese Eigenschaft die Id des Benutzers, der Zustimmung erteilt und gilt nur für diesen Benutzer an.</span><span class="sxs-lookup"><span data-stu-id="f0e38-128">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="f0e38-129">resourceId</span><span class="sxs-lookup"><span data-stu-id="f0e38-129">resourceId</span></span>|<span data-ttu-id="f0e38-130">String</span><span class="sxs-lookup"><span data-stu-id="f0e38-130">String</span></span>| <span data-ttu-id="f0e38-131">Gibt die Id des Prinzipals Service Resource, der Zugriff gewährt wurde.</span><span class="sxs-lookup"><span data-stu-id="f0e38-131">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="f0e38-132">Bereich</span><span class="sxs-lookup"><span data-stu-id="f0e38-132">scope</span></span>|<span data-ttu-id="f0e38-133">String</span><span class="sxs-lookup"><span data-stu-id="f0e38-133">String</span></span>| <span data-ttu-id="f0e38-134">Gibt den Wert des Anspruchs [Bereich](/graph/permissions-reference) , der die Ressource Anwendung erwarten im Zugriffstoken OAuth 2.0 an.</span><span class="sxs-lookup"><span data-stu-id="f0e38-134">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="f0e38-135">Beispielsweise *User.Read*</span><span class="sxs-lookup"><span data-stu-id="f0e38-135">For example, *User.Read*</span></span> |
|<span data-ttu-id="f0e38-136">startTime</span><span class="sxs-lookup"><span data-stu-id="f0e38-136">startTime</span></span>|<span data-ttu-id="f0e38-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0e38-137">DateTimeOffset</span></span>| <span data-ttu-id="f0e38-138">Derzeit wird der Wert für die Startzeit ignoriert.</span><span class="sxs-lookup"><span data-stu-id="f0e38-138">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f0e38-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f0e38-139">Relationships</span></span>
<span data-ttu-id="f0e38-140">Keine</span><span class="sxs-lookup"><span data-stu-id="f0e38-140">None</span></span>


## <a name="methods"></a><span data-ttu-id="f0e38-141">Methoden</span><span class="sxs-lookup"><span data-stu-id="f0e38-141">Methods</span></span>

| <span data-ttu-id="f0e38-142">Methode</span><span class="sxs-lookup"><span data-stu-id="f0e38-142">Method</span></span>           | <span data-ttu-id="f0e38-143">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f0e38-143">Return Type</span></span>    |<span data-ttu-id="f0e38-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0e38-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f0e38-145">Abrufen von oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="f0e38-145">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="f0e38-146">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="f0e38-146">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="f0e38-147">Lesen Sie Eigenschaften und Beziehungen des oAuth2PermissionGrant-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f0e38-147">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="f0e38-148">Liste oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="f0e38-148">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="f0e38-149">[oAuth2PermissionGrant](oauth2permissiongrant.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="f0e38-149">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="f0e38-150">Abrufen einer Liste von oauth2PermissionGrant-Objekten.</span><span class="sxs-lookup"><span data-stu-id="f0e38-150">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="f0e38-151">OAuth2PermissionGrant aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f0e38-151">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="f0e38-152">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="f0e38-152">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="f0e38-153">OAuth2PermissionGrant-Objekt zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="f0e38-153">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="f0e38-154">OAuth2PermissionGrant löschen</span><span class="sxs-lookup"><span data-stu-id="f0e38-154">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="f0e38-155">Keine</span><span class="sxs-lookup"><span data-stu-id="f0e38-155">None</span></span> |<span data-ttu-id="f0e38-156">OAuth2PermissionGrant-Objekt zu löschen.</span><span class="sxs-lookup"><span data-stu-id="f0e38-156">Delete oAuth2PermissionGrant object.</span></span> |

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
