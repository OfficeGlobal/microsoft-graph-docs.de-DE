---
title: Ressourcentyp requiredResourceAccess
description: Gibt den Satz von OAuth 2.0 berechtigungsbereiche und app-Rollen unter der angegebenen Ressource, der eine Anwendung Zugriff auf erforderlich ist. Die angegebene OAuth 2.0 berechtigungsbereiche möglicherweise beim von Clientanwendungen (über die **RequiredResourceAccess** -Auflistung) angefordert werden eine Anwendung Resource aufrufen. Die **RequiredResourceAccess** -Eigenschaft der Anwendung Entität ist eine Auflistung von **ReqiredResourceAccess**.
localization_priority: Normal
ms.openlocfilehash: a2c7e337bbe441275f395c2333b8cee918e6b9da
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512969"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="72e13-105">Ressourcentyp requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="72e13-105">requiredResourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72e13-106">Gibt den Satz von OAuth 2.0 berechtigungsbereiche und app-Rollen unter der angegebenen Ressource, der eine Anwendung Zugriff auf erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="72e13-106">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="72e13-107">Die angegebene OAuth 2.0 berechtigungsbereiche möglicherweise beim von Clientanwendungen (über die **RequiredResourceAccess** -Auflistung) angefordert werden eine Anwendung Resource aufrufen.</span><span class="sxs-lookup"><span data-stu-id="72e13-107">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="72e13-108">Die **RequiredResourceAccess** -Eigenschaft der [Anwendung](application.md) Entität ist eine Auflistung von **ReqiredResourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="72e13-108">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="72e13-109">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="72e13-109">JSON representation</span></span>

<span data-ttu-id="72e13-110">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="72e13-110">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}-->

```json
{
  "resourceAccess": [{"@odata.type": "microsoft.graph.resourceAccess"}],
  "resourceAppId": "string"
}

```
## <a name="properties"></a><span data-ttu-id="72e13-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="72e13-111">Properties</span></span>
| <span data-ttu-id="72e13-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="72e13-112">Property</span></span>     | <span data-ttu-id="72e13-113">Typ</span><span class="sxs-lookup"><span data-stu-id="72e13-113">Type</span></span>   |<span data-ttu-id="72e13-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72e13-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72e13-115">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="72e13-115">resourceAccess</span></span>|<span data-ttu-id="72e13-116">[ResourceAccess](resourceaccess.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="72e13-116">[ResourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="72e13-117">Die Liste der OAuth2.0 berechtigungsbereiche und app-Rollen, die die Anwendung aus der angegebenen Ressource erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="72e13-117">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="72e13-118">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="72e13-118">resourceAppId</span></span>|<span data-ttu-id="72e13-119">String</span><span class="sxs-lookup"><span data-stu-id="72e13-119">String</span></span>|<span data-ttu-id="72e13-120">Der eindeutige Bezeichner für die Ressource, der Zugriff auf für die Anwendung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="72e13-120">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="72e13-121">Dies sollte der **AppId** für die Zielanwendung für die Ressource deklarierten gleich sein.</span><span class="sxs-lookup"><span data-stu-id="72e13-121">This should be equal to the **appId** declared on the target resource application.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/requiredresourceaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
