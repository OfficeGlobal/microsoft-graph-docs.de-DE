---
title: Ressourcentyp requiredResourceAccess
description: Gibt den Satz von OAuth 2.0 berechtigungsbereiche und app-Rollen unter der angegebenen Ressource, der eine Anwendung Zugriff auf erforderlich ist. Die angegebene OAuth 2.0 berechtigungsbereiche möglicherweise beim von Clientanwendungen (über die **RequiredResourceAccess** -Auflistung) angefordert werden eine Anwendung Resource aufrufen. Die **RequiredResourceAccess** -Eigenschaft der Anwendung Entität ist eine Auflistung von **ReqiredResourceAccess**.
ms.openlocfilehash: 937557f2f078ade1b336cfd00cd128d428d59cbb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064189"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="00ee8-105">Ressourcentyp requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="00ee8-105">requiredResourceAccess resource type</span></span>

> <span data-ttu-id="00ee8-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="00ee8-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00ee8-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="00ee8-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00ee8-108">Gibt den Satz von OAuth 2.0 berechtigungsbereiche und app-Rollen unter der angegebenen Ressource, der eine Anwendung Zugriff auf erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="00ee8-108">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="00ee8-109">Die angegebene OAuth 2.0 berechtigungsbereiche möglicherweise beim von Clientanwendungen (über die **RequiredResourceAccess** -Auflistung) angefordert werden eine Anwendung Resource aufrufen.</span><span class="sxs-lookup"><span data-stu-id="00ee8-109">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="00ee8-110">Die **RequiredResourceAccess** -Eigenschaft der [Anwendung](application.md) Entität ist eine Auflistung von **ReqiredResourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="00ee8-110">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="00ee8-111">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="00ee8-111">JSON representation</span></span>

<span data-ttu-id="00ee8-112">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="00ee8-112">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="00ee8-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="00ee8-113">Properties</span></span>
| <span data-ttu-id="00ee8-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="00ee8-114">Property</span></span>     | <span data-ttu-id="00ee8-115">Typ</span><span class="sxs-lookup"><span data-stu-id="00ee8-115">Type</span></span>   |<span data-ttu-id="00ee8-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00ee8-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00ee8-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="00ee8-117">resourceAccess</span></span>|<span data-ttu-id="00ee8-118">[ResourceAccess](resourceaccess.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="00ee8-118">[ResourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="00ee8-119">Die Liste der OAuth2.0 berechtigungsbereiche und app-Rollen, die die Anwendung aus der angegebenen Ressource erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="00ee8-119">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="00ee8-120">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="00ee8-120">resourceAppId</span></span>|<span data-ttu-id="00ee8-121">String</span><span class="sxs-lookup"><span data-stu-id="00ee8-121">String</span></span>|<span data-ttu-id="00ee8-122">Der eindeutige Bezeichner für die Ressource, der Zugriff auf für die Anwendung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="00ee8-122">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="00ee8-123">Dies sollte der **AppId** für die Zielanwendung für die Ressource deklarierten gleich sein.</span><span class="sxs-lookup"><span data-stu-id="00ee8-123">This should be equal to the **appId** declared on the target resource application.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
