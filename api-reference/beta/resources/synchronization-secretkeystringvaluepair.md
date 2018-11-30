---
title: Ressourcentyp synchronizationSecretKeyStringValuePair
description: 'Stellt einen einzelnen geheimen Wert dar. '
ms.openlocfilehash: 31aa5d983a0117591d3be75939b2c881a9782e7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065660"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="1cb73-103">Ressourcentyp synchronizationSecretKeyStringValuePair</span><span class="sxs-lookup"><span data-stu-id="1cb73-103">synchronizationSecretKeyStringValuePair resource type</span></span>

> <span data-ttu-id="1cb73-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1cb73-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1cb73-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1cb73-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1cb73-106">Stellt einen einzelnen geheimen Wert dar.</span><span class="sxs-lookup"><span data-stu-id="1cb73-106">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="1cb73-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1cb73-107">Properties</span></span>
| <span data-ttu-id="1cb73-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1cb73-108">Property</span></span>     | <span data-ttu-id="1cb73-109">Typ</span><span class="sxs-lookup"><span data-stu-id="1cb73-109">Type</span></span>   |<span data-ttu-id="1cb73-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1cb73-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cb73-111">Key</span><span class="sxs-lookup"><span data-stu-id="1cb73-111">key</span></span>|<span data-ttu-id="1cb73-112">String</span><span class="sxs-lookup"><span data-stu-id="1cb73-112">String</span></span>| <span data-ttu-id="1cb73-113">Mögliche Werte sind: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken` , `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span><span class="sxs-lookup"><span data-stu-id="1cb73-113">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span></span>|
|<span data-ttu-id="1cb73-114">Wert</span><span class="sxs-lookup"><span data-stu-id="1cb73-114">value</span></span>|<span data-ttu-id="1cb73-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1cb73-115">String</span></span>|<span data-ttu-id="1cb73-116">Der Wert des geheimen Schlüssels.</span><span class="sxs-lookup"><span data-stu-id="1cb73-116">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1cb73-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1cb73-117">JSON representation</span></span>

<span data-ttu-id="1cb73-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1cb73-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSecretKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->