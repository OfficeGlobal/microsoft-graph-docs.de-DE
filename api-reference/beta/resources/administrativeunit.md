---
title: Ressourcentyp administrativeUnit
description: Eine administrative Einheit enthält einen konzeptionellen Container für Benutzer- und Verzeichnisobjekte. Verwenden von administrativen Einheiten, ein Unternehmensadministrator delegieren kann jetzt administrative Aufgaben zum Verwalten von Benutzern und Gruppen innerhalb oder auf eine administrative Einheit an einen Administrator regionalen oder auf Abteilungsebene bereichsbezogenen.
localization_priority: Normal
ms.openlocfilehash: 523214d7bd319d940f042d461b4903ff1f1475e1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845409"
---
# <a name="administrativeunit-resource-type"></a>Ressourcentyp administrativeUnit

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Eine administrative Einheit enthält einen konzeptionellen Container für Benutzer- und Verzeichnisobjekte. Verwenden von administrativen Einheiten, ein Unternehmensadministrator delegieren kann jetzt administrative Aufgaben zum Verwalten von Benutzern und Gruppen innerhalb oder auf eine administrative Einheit an einen Administrator regionalen oder auf Abteilungsebene bereichsbezogenen.

Sehen wir uns ein Beispiel. Angenommen Sie, Contoso Corp aus zwei Abschnitte - Division Süd und eine Division Nord besteht. Verzeichnis Rollen bei Contoso sind auf den gesamten Mandanten beschränkt. Kelly, ein Administrator von Contoso Unternehmen, möchte Verwaltungsaufgaben delegieren, aber die Division Süd oder die Division Nord festlegen.  Kelly kann *Süd Admistrative Einheit* erstellen und alle Süd Benutzer in dieser administrative Einheit platzieren.  Ebenso kann Kelly eine *Nord administrative Einheit*erstellen.  Nun können Kelly, starten Sie Delegieren von Verwaltungsaufgaben an andere Personen, aber in die neuen administrativen Einheiten **bezogenen** er erstellt wird. Kelly platziert zur Verfügung, in eine *Helpdeskadministrator* Rolle **als Bereich** der *Süd administrative Einheit*.  Dadurch wird zur Verfügung Kennwort des Benutzers, aber nur, wenn diese Benutzer in der *Süd administrative Einheit*sind zurücksetzen.  In ähnlicher Weise platziert Kelly Dave in einen *Benutzer Kontoadministrator* Rolle **bezogenen** zur *Nord administrative Einheit*.  Dadurch können Benutzer aktualisieren, Zuweisen von Lizenzen und Zurücksetzen des Kennworts des Benutzers, aber nur, wenn die Benutzer in der *Nord administrative Einheit sind*Dave. Video mit einer Übersicht finden Sie unter [Einführung in Azure Active Directory Administrative Einheiten](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units).

Diese Ressource ermöglicht es Ihnen, benutzerdefinierten Eigenschaften mithilfe von [Erweiterungen](/graph/extensibility-overview) eigene Daten hinzuzufügen.

Dieses Thema enthält eine Beschreibung der deklarierte Eigenschaften und Navigationseigenschaften verfügbar gemacht werden, durch die AdministrativeUnit-Entität als auch die Vorgänge und Funktionen, die für die Ressource AdministrativeUnits aufgerufen werden können.


## <a name="methods"></a>Methoden

| Methode   | Rückgabetyp | Beschreibung |
|:---------------|:--------|:----------|
|[Erstellen von administrativeUnit](../api/administrativeunit-post-administrativeunits.md) | [administrativeUnit](administrativeunit.md) | Erstellen Sie eine neue administrative Einheit.|
|[Liste administrativeUnits](../api/administrativeunit-list.md) | [AdministrativeUnit](administrativeunit.md) -Auflistung |Aller AdministrativeUnits-Listeneigenschaften.|
|[AdministrativeUnit abrufen](../api/administrativeunit-get.md) | [administrativeUnit](administrativeunit.md) |Lesen Sie Eigenschaften und die Beziehungen eines bestimmten AdministrativeUnit-Objekts.|
|[AdminstrativeUnit aktualisieren](../api/administrativeunit-update.md) | [administrativeUnit](administrativeunit.md)  |AdministrativeUnit-Objekt zu aktualisieren. |
|[AdminstrativeUnit löschen](../api/administrativeunit-delete.md) | Keine |AdministrativeUnit-Objekt zu löschen. |
|[Ein Mitglied hinzufügen](../api/administrativeunit-post-members.md) |[directoryObject](directoryobject.md)| Fügen Sie ein Mitglied (Benutzer oder Gruppe).|
|[Mitglieder auflisten](../api/administrativeunit-list-members.md) |[directoryObject](directoryobject.md)-Sammlung| Rufen Sie die Liste der Elemente (Benutzer und Gruppen).|
|[Abrufen eines Elements](../api/administrativeunit-get-members.md) |[directoryObject](directoryobject.md)| Rufen Sie ein bestimmtes Element.|
|[Mitglied entfernen](../api/administrativeunit-delete-members.md) |[directoryObject](directoryobject.md)| Entfernen eines Mitglieds.|
|[Gültigkeitsbereich der Rolle hinzufügen](../api/administrativeunit-post-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Fügen Sie ein Mitglied einer bezogenen-Rolle hinzu.|
|[Mitglieder der Liste bezogenen-Rolle](../api/administrativeunit-list-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)-Sammlung| Rufen Sie die Liste der Administratoren bezogenen-Rolle.|
|[Ein Mitglied einer bezogenen Rolle abrufen](../api/administrativeunit-get-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Rufen Sie ein bestimmtes Element bezogenen-Rolle.|
|[Entfernen eines Mitglieds bezogenen-Rolle](../api/administrativeunit-delete-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Entfernen Sie ein Mitglied einer bezogenen-Rolle.|
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften zu einer neuen oder vorhandenen Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Dient zum Abrufen einer offenen Erweiterung, die durch den Erweiterungsnamen identifiziert wird.|
|**Schemaerweiterungen**| | |
|[Schemaerweiterungswerte hinzufügen](/graph/extensibility-schema-groups) || Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|description|string|Eine optionale Beschreibung für die administrative Einheit.|
|displayName|string|Der Anzeigename für die administrative Einheit.|
|id|string|Eindeutiger Bezeichner für die administrative Einheit. Schreibgeschützt.|
|visibility|string|Steuert, ob die administrative Einheit und seine Member ausgeblendet sind oder öffentlich. Kann auf HiddenMembership oder öffentlichen festgelegt werden. Wenn nicht festgelegt, Standardverhalten öffentlich. Bei Festlegung auf HiddenMembership, können nur Mitglieder der administrative Einheit andere Mitglieder der administrative Einheit anbieten.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Erweiterungen|[extension](extension.md)-Sammlung|Die Auflistung der open-Erweiterungen für diese Administrative Einheit definiert. Lässt Nullwerte zu.|
|Elemente|[directoryObject](directoryobject.md)-Sammlung|Benutzer und Gruppen, die Mitglieder dieser Adminsitrative Einheit sind. HTTP-Methoden: Abrufen (Listenmitglieder) POST (Hinzufügen von Mitgliedern), DELETE (Entfernen von Mitgliedern).|
|scopedRoleMembers|[scopedRoleMembership](scopedrolemembership.md)-Sammlung| Bezogenen Rolle Mitglieder dieser Administrative Einheit.  HTTP-Methoden: Abrufen (Liste ScopedRoleMemberships), POST (ScopedRoleMembership hinzufügen), DELETE (Remove ScopedRoleMembership). |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.administrativeUnit"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "visibility": "string"
}

```


## <a name="see-also"></a>Weitere Artikel

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](/graph/extensibility-open-users)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "administrativeUnit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
