---
title: passwordProfile-Ressourcentyp
description: Enthält das einem Benutzer zugewiesene Kennwortprofil. Die **passwordProfile**-Eigenschaft der user-Entität ist ein **asswordProfile**-Objekt.
localization_priority: Normal
ms.openlocfilehash: 11930b046fafaf89f8db751891b9b7f2f72fd99d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839004"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="77b22-104">passwordProfile-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="77b22-104">passwordProfile resource type</span></span>

> <span data-ttu-id="77b22-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="77b22-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77b22-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77b22-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="77b22-p103">Enthält das einem Benutzer zugewiesene Kennwortprofil. Die **passwordProfile**-Eigenschaft der [user](user.md)-Entität ist ein **asswordProfile**-Objekt.</span><span class="sxs-lookup"><span data-stu-id="77b22-p103">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="77b22-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="77b22-109">Properties</span></span>
| <span data-ttu-id="77b22-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77b22-110">Property</span></span>     | <span data-ttu-id="77b22-111">Typ</span><span class="sxs-lookup"><span data-stu-id="77b22-111">Type</span></span>   |<span data-ttu-id="77b22-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77b22-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77b22-113">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="77b22-113">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="77b22-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="77b22-114">Boolean</span></span>| <span data-ttu-id="77b22-115">Wenn **true**, bei der nächsten Anmeldung, die Benutzer ihre Kennwörter ändern müssen.</span><span class="sxs-lookup"><span data-stu-id="77b22-115">If **true**, at next sign-in, the user must change their password.</span></span> <span data-ttu-id="77b22-116">Nach der kennwortänderung einer diese Eigenschaft wird automatisch auf zurückgesetzt \***"false"**.</span><span class="sxs-lookup"><span data-stu-id="77b22-116">After a password change, this property will be automatically reset to \***false**.</span></span> <span data-ttu-id="77b22-117">Wenn dies nicht festgelegt, Standard ist **false**.</span><span class="sxs-lookup"><span data-stu-id="77b22-117">If not set, default is **false**.</span></span> |
|<span data-ttu-id="77b22-118">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="77b22-118">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="77b22-119">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="77b22-119">Boolean</span></span>| <span data-ttu-id="77b22-120">Wenn **true**, bei der nächsten Anmeldung, die Benutzer ausführen müssen, erzwungen eine mehrstufige Authentifizierung (mehrstufiger Authentifizierung das), bevor Sie ihr Kennwort ändern.</span><span class="sxs-lookup"><span data-stu-id="77b22-120">If **true**, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="77b22-121">Das Verhalten ist identisch mit **ForceChangePasswordNextSignIn** , mit der Ausnahme, dass der Benutzer aufgefordert wird, eine mehrstufige Authentifizierung zuerst ausführen, bevor das Kennwort ändern.</span><span class="sxs-lookup"><span data-stu-id="77b22-121">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="77b22-122">Nach dem Kennwort zu ändern wird diese Eigenschaft automatisch auf **false**zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="77b22-122">After a password change, this property will be automatically reset to **false**.</span></span> <span data-ttu-id="77b22-123">Wenn dies nicht festgelegt, Standard ist **false**.</span><span class="sxs-lookup"><span data-stu-id="77b22-123">If not set, default is **false**.</span></span> |
|<span data-ttu-id="77b22-124">password</span><span class="sxs-lookup"><span data-stu-id="77b22-124">password</span></span>|<span data-ttu-id="77b22-125">String</span><span class="sxs-lookup"><span data-stu-id="77b22-125">String</span></span>|<span data-ttu-id="77b22-p106">Das Kennwort für den Benutzer.. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Sie kann aktualisiert werden, aber der Benutzer muss das Kennwort bei der nächsten Anmeldung ändern. Das Kennwort muss den Mindestanforderungen entsprechen, wie von der **passwordPolicies**-Eigenschaft des Benutzers angegeben.  Standardmäßig ist ein sicheres Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="77b22-p106">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77b22-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="77b22-131">JSON representation</span></span>

<span data-ttu-id="77b22-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="77b22-132">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordprofile"
}-->

```json
{
  "forceChangePasswordNextSignIn": true,
  "forceChangePasswordNextSignInWithMfa": false,
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
