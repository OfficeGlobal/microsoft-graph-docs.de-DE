---
title: passwordProfile-Ressourcentyp
description: Enthält das einem Benutzer zugewiesene Kennwortprofil. Die **passwordProfile**-Eigenschaft der user-Entität ist ein **passwordProfile**-Objekt.
localization_priority: Normal
ms.openlocfilehash: 3caff59c8fd0838b91f9fdfb79bdbb154aa83b9f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642898"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="2c24a-104">passwordProfile-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2c24a-104">passwordProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c24a-p102">Enthält das einem Benutzer zugewiesene Kennwortprofil. Die **passwordProfile**-Eigenschaft der [user](user.md)-Entität ist ein **asswordProfile**-Objekt.</span><span class="sxs-lookup"><span data-stu-id="2c24a-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="2c24a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2c24a-107">Properties</span></span>
| <span data-ttu-id="2c24a-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2c24a-108">Property</span></span>     | <span data-ttu-id="2c24a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="2c24a-109">Type</span></span>   |<span data-ttu-id="2c24a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2c24a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c24a-111">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="2c24a-111">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="2c24a-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c24a-112">Boolean</span></span>| <span data-ttu-id="2c24a-113">Wenn **true**, bei der nächsten Anmeldung, die Benutzer ihre Kennwörter ändern müssen.</span><span class="sxs-lookup"><span data-stu-id="2c24a-113">If **true**, at next sign-in, the user must change their password.</span></span> <span data-ttu-id="2c24a-114">Nach der kennwortänderung einer diese Eigenschaft wird automatisch auf zurückgesetzt \***"false"**.</span><span class="sxs-lookup"><span data-stu-id="2c24a-114">After a password change, this property will be automatically reset to \***false**.</span></span> <span data-ttu-id="2c24a-115">Wenn sie nicht festgelegt ist, wird standardmäßig **false** verwendet.</span><span class="sxs-lookup"><span data-stu-id="2c24a-115">If not set, default is **false**.</span></span> |
|<span data-ttu-id="2c24a-116">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="2c24a-116">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="2c24a-117">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2c24a-117">Boolean</span></span>| <span data-ttu-id="2c24a-118">Bei **true** muss der Benutzer bei der nächsten Anmeldung eine mehrstufige Authentifizierung ausführen, bevor er aufgefordert wird, sein Kennwort zu ändern.</span><span class="sxs-lookup"><span data-stu-id="2c24a-118">If **true**, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="2c24a-119">Das Verhalten ist identisch mit **forceChangePasswordNextSignIn** mit dem Unterschied, dass der Benutzer vor dem Ändern des Kennworts zuerst eine mehrstufige Authentifizierung ausführen muss.</span><span class="sxs-lookup"><span data-stu-id="2c24a-119">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="2c24a-120">Nach dem Ändern des Kennworts wird diese Eigenschaft automatisch auf **false** zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="2c24a-120">After a password change, this property will be automatically reset to **false**.</span></span> <span data-ttu-id="2c24a-121">Wenn sie nicht festgelegt ist, wird standardmäßig **false** verwendet.</span><span class="sxs-lookup"><span data-stu-id="2c24a-121">If not set, default is **false**.</span></span> |
|<span data-ttu-id="2c24a-122">password</span><span class="sxs-lookup"><span data-stu-id="2c24a-122">password</span></span>|<span data-ttu-id="2c24a-123">String</span><span class="sxs-lookup"><span data-stu-id="2c24a-123">String</span></span>|<span data-ttu-id="2c24a-p105">Das Kennwort für den Benutzer.. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Sie kann aktualisiert werden, aber der Benutzer muss das Kennwort bei der nächsten Anmeldung ändern. Das Kennwort muss den Mindestanforderungen entsprechen, wie von der **passwordPolicies**-Eigenschaft des Benutzers angegeben.  Standardmäßig ist ein sicheres Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2c24a-p105">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2c24a-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2c24a-129">JSON representation</span></span>

<span data-ttu-id="2c24a-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2c24a-130">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/passwordprofile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
