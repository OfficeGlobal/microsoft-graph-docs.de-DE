---
title: passwordProfile-Ressourcentyp
description: Enthält das einem Benutzer zugewiesene Kennwortprofil. Die **passwordProfile**-Eigenschaft der user-Entität ist ein **passwordProfile**-Objekt.
localization_priority: Priority
ms.openlocfilehash: cea8dcc114cb599a2d857ced67ac25c9eb275497
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526025"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="ef9e5-104">passwordProfile-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ef9e5-104">passwordProfile resource type</span></span>

<span data-ttu-id="ef9e5-p102">Enthält das einem Benutzer zugewiesene Kennwortprofil. Die **passwordProfile**-Eigenschaft der [user](user.md)-Entität ist ein **asswordProfile**-Objekt.</span><span class="sxs-lookup"><span data-stu-id="ef9e5-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="ef9e5-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ef9e5-107">Properties</span></span>
| <span data-ttu-id="ef9e5-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ef9e5-108">Property</span></span>     | <span data-ttu-id="ef9e5-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ef9e5-109">Type</span></span>   |<span data-ttu-id="ef9e5-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ef9e5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef9e5-111">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="ef9e5-111">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="ef9e5-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef9e5-112">Boolean</span></span>| <span data-ttu-id="ef9e5-113">**true**, wenn der Benutzer sein Kennwort bei der nächsten Anmeldung ändern muss, andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="ef9e5-113">**true** if the user must change her password on the next login; otherwise **false**.</span></span> |
|<span data-ttu-id="ef9e5-114">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="ef9e5-114">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="ef9e5-115">Boolesch</span><span class="sxs-lookup"><span data-stu-id="ef9e5-115">Boolean</span></span>| <span data-ttu-id="ef9e5-116">Bei **true** muss der Benutzer bei der nächsten Anmeldung eine mehrstufige Authentifizierung ausführen, bevor er aufgefordert wird, sein Kennwort zu ändern.</span><span class="sxs-lookup"><span data-stu-id="ef9e5-116">If **true**, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="ef9e5-117">Das Verhalten ist identisch mit **forceChangePasswordNextSignIn** mit dem Unterschied, dass der Benutzer vor dem Ändern des Kennworts zuerst eine mehrstufige Authentifizierung ausführen muss.</span><span class="sxs-lookup"><span data-stu-id="ef9e5-117">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="ef9e5-118">Nach dem Ändern des Kennworts wird diese Eigenschaft automatisch auf **false** zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="ef9e5-118">After a password change, this property will be automatically reset to **false**.</span></span> <span data-ttu-id="ef9e5-119">Wenn sie nicht festgelegt ist, wird standardmäßig **false** verwendet.</span><span class="sxs-lookup"><span data-stu-id="ef9e5-119">If not set, default is **false**.</span></span> |
|<span data-ttu-id="ef9e5-120">password</span><span class="sxs-lookup"><span data-stu-id="ef9e5-120">password</span></span>|<span data-ttu-id="ef9e5-121">String</span><span class="sxs-lookup"><span data-stu-id="ef9e5-121">String</span></span>|<span data-ttu-id="ef9e5-p104">Das Kennwort für den Benutzer.. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Sie kann aktualisiert werden, aber der Benutzer muss das Kennwort bei der nächsten Anmeldung ändern. Das Kennwort muss den Mindestanforderungen entsprechen, wie von der **passwordPolicies**-Eigenschaft des Benutzers angegeben.  Standardmäßig ist ein sicheres Kennwort erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ef9e5-p104">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ef9e5-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ef9e5-127">JSON representation</span></span>

<span data-ttu-id="ef9e5-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ef9e5-128">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordProfile"
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
