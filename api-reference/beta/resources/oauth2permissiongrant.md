---
title: Ressourcentyp oAuth2PermissionGrant
description: Stellt die OAuth 2.0-Bereiche (delegierten Berechtigungen) zu einer Anwendung (dargestellt durch ein Dienstprinzipal) erteilt wurden im Rahmen des Prozesses Zustimmung Benutzer oder Administrator an.
localization_priority: Normal
ms.openlocfilehash: 835e4a2c1a8d19c9c21e706adbf2f10a6a505bb3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884448"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="f0990-103">Ressourcentyp oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="f0990-103">oAuth2PermissionGrant resource type</span></span>

> <span data-ttu-id="f0990-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f0990-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0990-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f0990-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f0990-106">Stellt die OAuth 2.0-Bereiche (delegierten Berechtigungen) zu einer Anwendung (dargestellt durch ein Dienstprinzipal) erteilt wurden im Rahmen des Prozesses Zustimmung Benutzer oder Administrator an.</span><span class="sxs-lookup"><span data-stu-id="f0990-106">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0990-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f0990-107">JSON representation</span></span>

<span data-ttu-id="f0990-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f0990-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="f0990-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f0990-109">Properties</span></span>
| <span data-ttu-id="f0990-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f0990-110">Property</span></span>     | <span data-ttu-id="f0990-111">Typ</span><span class="sxs-lookup"><span data-stu-id="f0990-111">Type</span></span>   |<span data-ttu-id="f0990-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0990-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0990-113">clientId</span><span class="sxs-lookup"><span data-stu-id="f0990-113">clientId</span></span>|<span data-ttu-id="f0990-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f0990-114">String</span></span>| <span data-ttu-id="f0990-115">Die Id des Prinzipals Dienst gewährt Ihr Einverständnis der Benutzer Identitätswechsel für den Zugriff auf die Ressource (dargestellt durch die ResourceId-Eigenschaft).</span><span class="sxs-lookup"><span data-stu-id="f0990-115">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="f0990-116">consentType</span><span class="sxs-lookup"><span data-stu-id="f0990-116">consentType</span></span>|<span data-ttu-id="f0990-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f0990-117">String</span></span>| <span data-ttu-id="f0990-118">Gibt an, ob Zustimmung vom Administrator (im Namen der Organisation) oder von einer Person zur Verfügung gestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="f0990-118">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="f0990-119">Die möglichen Werte sind *AllPrincipals* oder *Prinzipal*.</span><span class="sxs-lookup"><span data-stu-id="f0990-119">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="f0990-120">expiryTime</span><span class="sxs-lookup"><span data-stu-id="f0990-120">expiryTime</span></span>|<span data-ttu-id="f0990-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0990-121">DateTimeOffset</span></span>| <span data-ttu-id="f0990-122">Derzeit ist der Ablauf Time-Wert ignoriert.</span><span class="sxs-lookup"><span data-stu-id="f0990-122">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="f0990-123">id</span><span class="sxs-lookup"><span data-stu-id="f0990-123">id</span></span>|<span data-ttu-id="f0990-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f0990-124">String</span></span>| <span data-ttu-id="f0990-125">Eindeutiger Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="f0990-125">Unique identifier.</span></span> <span data-ttu-id="f0990-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f0990-126">Read-only.</span></span>|
|<span data-ttu-id="f0990-127">principalId</span><span class="sxs-lookup"><span data-stu-id="f0990-127">principalId</span></span>|<span data-ttu-id="f0990-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f0990-128">String</span></span>| <span data-ttu-id="f0990-129">Wenn ConsentType *AllPrincipals* ist dieser Wert ist null, und die Zustimmung gilt für alle Benutzer in der Organisation.</span><span class="sxs-lookup"><span data-stu-id="f0990-129">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="f0990-130">Wenn ConsentType *Prinzipal*ist, gibt diese Eigenschaft die Id des Benutzers, der Zustimmung erteilt und gilt nur für diesen Benutzer an.</span><span class="sxs-lookup"><span data-stu-id="f0990-130">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="f0990-131">resourceId</span><span class="sxs-lookup"><span data-stu-id="f0990-131">resourceId</span></span>|<span data-ttu-id="f0990-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f0990-132">String</span></span>| <span data-ttu-id="f0990-133">Gibt die Id des Prinzipals Service Resource, der Zugriff gewährt wurde.</span><span class="sxs-lookup"><span data-stu-id="f0990-133">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="f0990-134">scope</span><span class="sxs-lookup"><span data-stu-id="f0990-134">scope</span></span>|<span data-ttu-id="f0990-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f0990-135">String</span></span>| <span data-ttu-id="f0990-136">Gibt den Wert des Anspruchs [Bereich](/graph/permissions-reference) , der die Ressource Anwendung erwarten im Zugriffstoken OAuth 2.0 an.</span><span class="sxs-lookup"><span data-stu-id="f0990-136">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="f0990-137">Beispielsweise *User.Read*</span><span class="sxs-lookup"><span data-stu-id="f0990-137">For example, *User.Read*</span></span> |
|<span data-ttu-id="f0990-138">startTime</span><span class="sxs-lookup"><span data-stu-id="f0990-138">startTime</span></span>|<span data-ttu-id="f0990-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0990-139">DateTimeOffset</span></span>| <span data-ttu-id="f0990-140">Derzeit wird der Wert für die Startzeit ignoriert.</span><span class="sxs-lookup"><span data-stu-id="f0990-140">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f0990-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f0990-141">Relationships</span></span>
<span data-ttu-id="f0990-142">Keine</span><span class="sxs-lookup"><span data-stu-id="f0990-142">None</span></span>


## <a name="methods"></a><span data-ttu-id="f0990-143">Methoden</span><span class="sxs-lookup"><span data-stu-id="f0990-143">Methods</span></span>

| <span data-ttu-id="f0990-144">Methode</span><span class="sxs-lookup"><span data-stu-id="f0990-144">Method</span></span>           | <span data-ttu-id="f0990-145">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f0990-145">Return Type</span></span>    |<span data-ttu-id="f0990-146">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0990-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f0990-147">Abrufen von oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="f0990-147">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="f0990-148">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="f0990-148">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="f0990-149">Lesen Sie Eigenschaften und Beziehungen des oAuth2PermissionGrant-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f0990-149">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="f0990-150">Liste oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="f0990-150">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="f0990-151">[oAuth2PermissionGrant](oauth2permissiongrant.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f0990-151">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="f0990-152">Abrufen einer Liste von oauth2PermissionGrant-Objekten.</span><span class="sxs-lookup"><span data-stu-id="f0990-152">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="f0990-153">OAuth2PermissionGrant aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f0990-153">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="f0990-154">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="f0990-154">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="f0990-155">OAuth2PermissionGrant-Objekt zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="f0990-155">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="f0990-156">OAuth2PermissionGrant löschen</span><span class="sxs-lookup"><span data-stu-id="f0990-156">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="f0990-157">Keine</span><span class="sxs-lookup"><span data-stu-id="f0990-157">None</span></span> |<span data-ttu-id="f0990-158">OAuth2PermissionGrant-Objekt zu löschen.</span><span class="sxs-lookup"><span data-stu-id="f0990-158">Delete oAuth2PermissionGrant object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
