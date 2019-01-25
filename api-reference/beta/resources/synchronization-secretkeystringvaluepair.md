---
title: Ressourcentyp synchronizationSecretKeyStringValuePair
description: 'Stellt einen einzelnen geheimen Wert dar. '
localization_priority: Normal
ms.openlocfilehash: a937063ea04bd3726932e423a065026d51b05aa4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526067"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="20818-103">Ressourcentyp synchronizationSecretKeyStringValuePair</span><span class="sxs-lookup"><span data-stu-id="20818-103">synchronizationSecretKeyStringValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20818-104">Stellt einen einzelnen geheimen Wert dar.</span><span class="sxs-lookup"><span data-stu-id="20818-104">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="20818-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="20818-105">Properties</span></span>
| <span data-ttu-id="20818-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="20818-106">Property</span></span>     | <span data-ttu-id="20818-107">Typ</span><span class="sxs-lookup"><span data-stu-id="20818-107">Type</span></span>   |<span data-ttu-id="20818-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="20818-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20818-109">Key</span><span class="sxs-lookup"><span data-stu-id="20818-109">key</span></span>|<span data-ttu-id="20818-110">String</span><span class="sxs-lookup"><span data-stu-id="20818-110">String</span></span>| <span data-ttu-id="20818-111">Mögliche Werte sind: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken` , `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span><span class="sxs-lookup"><span data-stu-id="20818-111">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span></span>|
|<span data-ttu-id="20818-112">Wert</span><span class="sxs-lookup"><span data-stu-id="20818-112">value</span></span>|<span data-ttu-id="20818-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="20818-113">String</span></span>|<span data-ttu-id="20818-114">Der Wert des geheimen Schlüssels.</span><span class="sxs-lookup"><span data-stu-id="20818-114">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20818-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="20818-115">JSON representation</span></span>

<span data-ttu-id="20818-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="20818-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
}-->

```json
{
  "key": "String",
  "value": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSecretKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-secretkeystringvaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
