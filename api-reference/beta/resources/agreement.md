---
title: Vereinbarung Ressourcentyp
description: Stellt einen Mandanten anpassbare Vertragsbedingungen verwenden, die erstellt und mit Azure Active Directory (AD Azure) verwaltet wird. Sie können die folgenden Methoden zum Erstellen und Verwalten des Azure Active Directory Ausdrücken verwenden Features gemäß Ihrem Szenario.
ms.openlocfilehash: 2e5c9087cd809f9c067150654d420fda533ca61b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060471"
---
# <a name="agreement-resource-type"></a>Vereinbarung Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt einen Mandanten anpassbare Vertragsbedingungen verwenden, die erstellt und mit Azure Active Directory (AD Azure) verwaltet wird. Sie können die folgenden Methoden zum Erstellen und Verwalten des [Azure Active Directory Ausdrücken verwenden Feature](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) entsprechend Ihrem Szenario.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp | Beschreibung |
|:-------------|:------------|:------------|
| [Vereinbarungen zur erstellen](../api/agreement-post-agreements.md) | [Vereinbarung](agreement.md) | Erstellen Sie eine neue Vereinbarung durch die Veröffentlichung auf der Vereinbarung-Auflistung. |
| [Vereinbarungen zur Liste](../api/agreement-list.md) | [Vereinbarung](agreement.md) -Auflistung | Rufen Sie eine Auflistung der Vereinbarung-Objekts. |
| [Abrufen der Vereinbarung](../api/agreement-get.md) | [Vereinbarung](agreement.md) | Lesen Sie Eigenschaften und Beziehungen eines Vereinbarung-Objekts. |
| [Vereinbarung aktualisieren](../api/agreement-update.md) | [Vereinbarung](agreement.md) | Ein Objekt zu aktualisieren. |
| [Vereinbarung löschen](../api/agreement-delete.md) | Keines | Ein Objekt zu löschen. |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|displayName|String|Der Anzeigename der Vereinbarung.|
|id|String| Schreibgeschützt.|
|isViewingBeforeAcceptanceRequired|Boolesch|Gibt an, ob der Benutzer zu erweitern und vor dem akzeptieren die Vereinbarung anzuzeigen.|

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
<!-- {
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->