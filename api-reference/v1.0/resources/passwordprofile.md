---
title: passwordProfile-Ressourcentyp
description: Enthält das einem Benutzer zugewiesene Kennwortprofil. Die **passwordProfile**-Eigenschaft der user-Entität ist ein **asswordProfile**-Objekt.
localization_priority: Priority
ms.openlocfilehash: 80d774906fb4897f57b943af827cfbc32e90511f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819663"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="a1663-104">passwordProfile-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a1663-104">passwordProfile resource type</span></span>

<span data-ttu-id="a1663-p102">Enthält das einem Benutzer zugewiesene Kennwortprofil. Die **passwordProfile**-Eigenschaft der [user](user.md)-Entität ist ein **asswordProfile**-Objekt.</span><span class="sxs-lookup"><span data-stu-id="a1663-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="a1663-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a1663-107">Properties</span></span>
| <span data-ttu-id="a1663-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a1663-108">Property</span></span>     | <span data-ttu-id="a1663-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a1663-109">Type</span></span>   |<span data-ttu-id="a1663-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1663-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1663-111">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="a1663-111">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="a1663-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1663-112">Boolean</span></span>| <span data-ttu-id="a1663-113">**true**, wenn der Benutzer sein Kennwort bei der nächsten Anmeldung ändern muss, andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="a1663-113">**true** if the user must change her password on the next login; otherwise **false**.</span></span> |
|<span data-ttu-id="a1663-114">password</span><span class="sxs-lookup"><span data-stu-id="a1663-114">password</span></span>|<span data-ttu-id="a1663-115">String</span><span class="sxs-lookup"><span data-stu-id="a1663-115">String</span></span>|<span data-ttu-id="a1663-p103">Das Kennwort für den Benutzer.. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Sie kann aktualisiert werden, aber der Benutzer muss das Kennwort bei der nächsten Anmeldung ändern. Das Kennwort muss den Mindestanforderungen entsprechen, wie von der **passwordPolicies**-Eigenschaft des Benutzers angegeben.  Standardmäßig ist ein sicheres Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a1663-p103">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a1663-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a1663-121">JSON representation</span></span>

<span data-ttu-id="a1663-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a1663-122">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordProfile"
}-->

```json
{
  "forceChangePasswordNextSignIn": true,
  "password": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
