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
# <a name="passwordprofile-resource-type"></a>passwordProfile-Ressourcentyp

Enthält das einem Benutzer zugewiesene Kennwortprofil. Die **passwordProfile**-Eigenschaft der [user](user.md)-Entität ist ein **asswordProfile**-Objekt.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|forceChangePasswordNextSignIn|Boolean| **true**, wenn der Benutzer sein Kennwort bei der nächsten Anmeldung ändern muss, andernfalls **false**. |
|forceChangePasswordNextSignInWithMfa|Boolesch| Bei **true** muss der Benutzer bei der nächsten Anmeldung eine mehrstufige Authentifizierung ausführen, bevor er aufgefordert wird, sein Kennwort zu ändern. Das Verhalten ist identisch mit **forceChangePasswordNextSignIn** mit dem Unterschied, dass der Benutzer vor dem Ändern des Kennworts zuerst eine mehrstufige Authentifizierung ausführen muss. Nach dem Ändern des Kennworts wird diese Eigenschaft automatisch auf **false** zurückgesetzt. Wenn sie nicht festgelegt ist, wird standardmäßig **false** verwendet. |
|password|String|Das Kennwort für den Benutzer.. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. Sie kann aktualisiert werden, aber der Benutzer muss das Kennwort bei der nächsten Anmeldung ändern. Das Kennwort muss den Mindestanforderungen entsprechen, wie von der **passwordPolicies**-Eigenschaft des Benutzers angegeben.  Standardmäßig ist ein sicheres Kennwort erforderlich.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

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
