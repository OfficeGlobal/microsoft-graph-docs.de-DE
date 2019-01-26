---
title: passwordProfile-Ressourcentyp
description: Enthält das einem Benutzer zugewiesene Kennwortprofil. Die **passwordProfile**-Eigenschaft der user-Entität ist ein **asswordProfile**-Objekt.
localization_priority: Normal
ms.openlocfilehash: a68cd61c7ab3fd1e62ca9bc889a6691068174dc6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574572"
---
# <a name="passwordprofile-resource-type"></a>passwordProfile-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Enthält das einem Benutzer zugewiesene Kennwortprofil. Die **passwordProfile**-Eigenschaft der [user](user.md)-Entität ist ein **asswordProfile**-Objekt.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|forceChangePasswordNextSignIn|Boolean| Wenn **true**, bei der nächsten Anmeldung, die Benutzer ihre Kennwörter ändern müssen. Nach der kennwortänderung einer diese Eigenschaft wird automatisch auf zurückgesetzt ***"false"**. Wenn dies nicht festgelegt, Standard ist **false**. |
|forceChangePasswordNextSignInWithMfa|Boolean| Wenn **true**, bei der nächsten Anmeldung, die Benutzer ausführen müssen, erzwungen eine mehrstufige Authentifizierung (mehrstufiger Authentifizierung das), bevor Sie ihr Kennwort ändern. Das Verhalten ist identisch mit **ForceChangePasswordNextSignIn** , mit der Ausnahme, dass der Benutzer aufgefordert wird, eine mehrstufige Authentifizierung zuerst ausführen, bevor das Kennwort ändern. Nach dem Kennwort zu ändern wird diese Eigenschaft automatisch auf **false**zurückgesetzt. Wenn dies nicht festgelegt, Standard ist **false**. |
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
