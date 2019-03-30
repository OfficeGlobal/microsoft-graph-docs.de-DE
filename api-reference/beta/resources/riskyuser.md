---
title: riskyUsers-Ressourcentyp
description: Stellt Azure AD-Benutzer dar, die gefährdet sind. Azure AD bewertet das Benutzer Risiko kontinuierlich anhand verschiedener Signale und des maschinellen Lernens. Diese API ermöglicht den programmgesteuerten Zugriff auf alle Risiko Benutzer in Azure AD.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3265ea40903ca2c5c10272f5df280bd3715af366
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/30/2019
ms.locfileid: "31003720"
---
# <a name="riskyusers-resource-type"></a>riskyUsers-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt Azure AD-Benutzer dar, die gefährdet sind. Azure AD bewertet das Benutzer Risiko kontinuierlich anhand verschiedener Signale und des maschinellen Lernens. Diese API ermöglicht den programmgesteuerten Zugriff auf alle Risiko Benutzer in Azure AD.

Weitere Informationen zu Risikoereignissen finden Sie unter [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).

>**Hinweis:** Die Verwendung der riskyUsers-API erfordert eine Azure AD Premium P2-Lizenz.

## <a name="methods"></a>Methoden

| Methode   | Rückgabetyp|Beschreibung|
|:---------------|:--------|:----------|
|[RiskyUsers aufListen](../api/riskyusers-list.md) | [riskyUsers](riskyUser.md) |AufListen von riskanten Benutzern und deren Eigenschaften.|
|[RiskyUsers abrufen](../api/riskyusers-get.md) | [riskyUsers](riskyUser.md)|Abrufen eines bestimmten riskanten Benutzers und seiner Eigenschaften.|
|[Bestätigen der riskyUsers kompromittiert](../api/riskyusers-confirmcompromised.md)|Bestätigen Sie einen riskanten Benutzer als kompromittiert.|
|[RiskyUsers schließen](../api/riskyusers-dismiss.md)|Schließen Sie das Risiko eines riskanten Benutzers ab.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|`id`|`string`|Eindeutige ID des gefährdeten Benutzers|
|`isDeleted`|`bool`|Gibt an, ob der Benutzer gelöscht wurde. Mögliche Werte sind: `true`,`false`|
|`isGuest`|`bool`|Gibt an, ob der Benutzer ein Gastbenutzer ist. Mögliche Werte sind: `true` und `false`. True, wenn die Identität des Benutzers außerhalb des Mandanten liegt. Dieser Benutzer kann ein B2B-oder ein B2C-Benutzer mit Identität in Azure AD, MSA oder Drittanbieter-Identitätsanbieter sein. False, wenn die Identität des Benutzers in Betracht gezogen wird|
|`isProcessing`|`bool`|Gibt an, wehther der riskante Status eines Benutzers vom Back-End verarbeitet wird.|
|`risk`|[Risiko](risk.md)|Riskanter Benutzerstatus|
|`riskLastUpdatedDateTime`|`datetime`|Datum und Uhrzeit der letzten Aktualisierung des Risiko Benutzer|
|`userDisplayName`|`string`|Riskanter Benutzeranzeigename|
|`userPrincipalName`|`string`|Riskanter Benutzerprinzipalname|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskyusers"
}-->

```json
{
 "id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isGuest": "boolean",
"isProcessing": "boolean",
"isDeleted": "boolean",
"risk": {"@odata.type": "microsoft.graph.risk"},
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
