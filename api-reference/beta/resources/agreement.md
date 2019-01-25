---
title: Vereinbarung Ressourcentyp
description: Stellt einen Mandanten anpassbare Vertragsbedingungen verwenden, die erstellt und mit Azure Active Directory (AD Azure) verwaltet wird. Sie können die folgenden Methoden zum Erstellen und Verwalten des Azure Active Directory Ausdrücken verwenden Features gemäß Ihrem Szenario.
localization_priority: Normal
ms.openlocfilehash: b253877f1bf82e4fbc61cebaef3c1bce208d9cca
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513851"
---
# <a name="agreement-resource-type"></a>Vereinbarung Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt einen Mandanten anpassbare Vertragsbedingungen verwenden, die erstellt und mit Azure Active Directory (AD Azure) verwaltet wird. Sie können die folgenden Methoden zum Erstellen und Verwalten des [Azure Active Directory Ausdrücken verwenden Feature](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) entsprechend Ihrem Szenario.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp | Beschreibung |
|:-------------|:------------|:------------|
| [Vereinbarungen zur erstellen](../api/agreement-post-agreements.md) | [Vereinbarung](agreement.md) | Erstellen Sie eine neue Vereinbarung durch die Veröffentlichung auf der Vereinbarung-Auflistung. |
| [Vereinbarungen zur Liste](../api/agreement-list.md) | [Vereinbarung](agreement.md) -Auflistung | Rufen Sie eine Auflistung der Vereinbarung-Objekts. |
| [Abrufen der Vereinbarung](../api/agreement-get.md) | [Vereinbarung](agreement.md) | Lesen Sie Eigenschaften und Beziehungen eines Vereinbarung-Objekts. |
| [Vereinbarung aktualisieren](../api/agreement-update.md) | [Vereinbarung](agreement.md) | Ein Objekt zu aktualisieren. |
| [Vereinbarung löschen](../api/agreement-delete.md) | Keine | Ein Objekt zu löschen. |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|displayName|Zeichenfolge|Der Anzeigename der Vereinbarung.|
|id|String| Schreibgeschützt.|
|isViewingBeforeAcceptanceRequired|Boolescher Wert|Gibt an, ob der Benutzer zu erweitern und vor dem akzeptieren die Vereinbarung anzuzeigen.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|files|[AgreementFile](agreementfile.md) -Auflistung|Schreibgeschützt. PDF-Dateien mit diesem Vertrag verknüpft sind.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreement"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "isViewingBeforeAcceptanceRequired": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/agreement.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
