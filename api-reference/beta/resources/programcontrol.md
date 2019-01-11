---
title: Ressourcentyp programControl
description: In Azure AD Access Feature überprüft, und das Programm Control-Objekt stellt ein Steuerelement, Verknüpfen einer Access-Überprüfung an ein Programm dar.
localization_priority: Normal
ms.openlocfilehash: ddf6e978277ca1801f9126597ac4b3561fe5bfb7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817822"
---
# <a name="programcontrol-resource-type"></a>Ressourcentyp programControl

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

In Azure AD [Access überprüft](accessreviews-root.md) Feature stellt das Programm Control-Objekt ein Steuerelement, Verknüpfen einer Access-Überprüfung mit einer Anwendung.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Erstellen von programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   Fügen Sie ein Programm ein ProgramControl hinzu.|
|[ProgramControl löschen](../api/programcontrol-delete.md) |     Keine.   |   Entfernen einer ProgramControl aus einem Programm.|
|[Liste programControls](../api/programcontrol-list.md) | [ProgramControl](programcontrol.md) -Auflistung| Von Listensteuerelementen in allen Programmen im Mandanten.|

## <a name="permissions"></a>Berechtigungen

|Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)     | ProgramControl.Read.All ProgramControl.ReadWrite.All |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
|Anwendung                            | Nicht unterstützt |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| `id`                     |`String`                | Die Feature-zugewiesenen Bezeichner der Verknüpfung zwischen Programm und Steuerelement                                      |
| `programId`              |`String`                | Die ProgramId des Programms dieses Steuerelement ist ein Teil der. Erforderliche auf erstellen.                            |
| `controlId`              |`String`                | Die ControlId des Steuerelements, insbesondere die eine Access-ID überprüfen. Erforderliche auf erstellen.                                                |
| `controlTypeId`          |`String`                | Die ProgramControlType identifiziert den Typ des programmfreigabesteuerung – beispielsweise ein Steuerelement verknüpfen mit Gast Access überprüft. Erforderliche auf erstellen. |
| `displayName`            |`String`                | Der Name des Steuerelements.                                                             |
| `status`                 |`String`                | Der Status des Lebenszyklus des Steuerelements.                                                 |
| `createdDateTime`        |`DateTimeOffset`        | Das Erstellungsdatum und die Uhrzeit des Steuerelements Programm.                                        |
| `owner`                  |[Benutzeridentität](useridentity.md)   | Der Benutzer, die das Programmsteuerelement erstellt.                                               |
| `resource`               |`programResource`       | Die Ressource, eine Gruppe oder eine app, Ziel dieses Programm Steuerelement Access überprüfen.                   |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| `program`                |[Programm](program.md)               | Die Anwendung dieses Steuerelement ist Bestandteil.                                                |

## <a name="see-also"></a>Siehe auch

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Liste ProgramControls eines Programms](../api/program-listcontrols.md) |      [ProgramControl](programcontrol.md) -Auflistung| Rufen Sie eine Auflistung der Steuerelemente eines Programms.|
|[Liste programControlTypes](../api/programcontroltype-list.md) | [ProgramControlType](programcontroltype.md) -Auflistung| Programm Steuerelement Listentypen. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControl"
}-->

```json
{
 "id": "string (identifier)",
 "programId": "string (identifier)",
 "controlId": "string (identifier)",
 "controlTypeId": "string (identifier)",
 "displayName": "string",
 "status": "string",
 "createdDateTime": "string (timestamp)",
 "owner": "microsoft.graph.userIdentity",
 "resource":"microsoft.graph.programResource"
}

```

## <a name="the-programresource-complex-type"></a>Den komplexen Typ programResource

Die Programm-Ressource, die ein Programm Control-Objekt enthaltenen ist eine Darstellung der einen Verweis auf ein Objekt, das das Ziel der Überprüfung Zugriff ist.

Dieser Typ erbt von `microsoft.graph.identity` und verfügt über eine zusätzliche Eigenschaft:

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| `type`               |`String`  | Der Typ der Ressource, zurück, der angibt, ob es sich um eine Gruppe oder eine app handelt. |     


<!-- {
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
