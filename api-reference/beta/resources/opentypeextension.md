---
title: openTypeExtension-Ressourcentyp (offene Erweiterungen)
description: Open-Erweiterungen (vormals Office 365 Daten Extensions) bieten eine einfache Möglichkeit nicht typisierte Eigenschaften auf eine Ressource in Microsoft Graph direkt hinzufügen.
ms.openlocfilehash: f28ab43ddb3fd55efbca6738a0369fde37c906db
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060805"
---
# <a name="opentypeextension-resource-type-open-extensions"></a>openTypeExtension-Ressourcentyp (offene Erweiterungen)

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Open-Erweiterungen (vormals Office 365 Daten Extensions) bieten eine einfache Möglichkeit nicht typisierte Eigenschaften auf eine Ressource in Microsoft Graph direkt hinzufügen.
Offiene Erweiterungen werden mithilfe der **openTypeExtension**-Ressource dargestellt. Alle offenen Erweiterungen, die einer Ressource hinzugefügt wurden, werden in der **extensions**-Navigationseigenschaft angezeigt, die vom abstrakten Typ [extension](extension.md) abgeleitet wird.  Jede Erweiterung weist eine **extensionName**-Eigenschaft auf, die die einzige vordefinierte, schreibbare Eigenschaft für alle Erweiterungen zusammen mit ihren benutzerdefinierten Daten ist. Um sicherzustellen, dass Erweiterungsnamen eindeutig sind, können Sie eine umgekehrtes DNS-Format (Domain Name System) verwenden, das _von Ihrer eigenen Domäne_, z. B. `Com.Contoso.ContactInfo`, abhängig ist. Verwenden Sie in Erweiterungsnamen auf keinen Fall die Microsoft-Domäne (`Com.Microsoft` oder `Com.OnMicrosoft`).

Beispiel für eine offene Erweiterung: [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](/graph/extensibility-open-users)

Offene Erweiterungen werden von den folgenden Ressourcen in den entsprechenden Versionen unterstützt: - Allgemein verfügbar (GA: /v1.0 und /beta) oder Vorschau (/beta).

| Ressource | Version |
|---------------|-------|
| [Administrative Einheit](administrativeunit.md)  | Nur Vorschau |
| [Kalenderereignis](event.md) | Allgemein verfügbar |
| [Kalenderereignis](event.md) für Gruppe | Allgemein verfügbar |
| Unterhaltungsthread der Gruppe [posten](post.md) | Allgemein verfügbar |
| [device](device.md) | Allgemein verfügbar |
| [group](group.md) | Allgemein verfügbar |
| [message](message.md) | Allgemein verfügbar |
| [organization](organization.md) | Allgemein verfügbar |
| [Privater Kontakt](contact.md) | Allgemein verfügbar |
| [user](user.md) | Allgemein verfügbar |

## <a name="outlook-specific-considerations"></a>Outlook-spezifische Aspekte

Jede open Erweiterung auf einer Outlook-Ressource (Ereignis, Nachricht oder persönlichen Kontakt) vorhanden ist in einem [MAPI benannte Eigenschaft](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx)gespeichert. Berücksichtigen Sie beim Erstellen von open-Erweiterungen für Outlook, dass MAPI benannte Eigenschaften sind eine begrenzte Ressource im Postfach des Benutzers. Wenn ein Benutzer benannte Eigenschaft Quota leer ist, können nicht Sie keine mehr benannten Eigenschaften für diesen Benutzer erstellen. Dies kann unerwartetes Verhalten von Clients führen, die benannte Eigenschaften-Funktion verwenden.

Wenden Sie die folgenden Richtlinien beim Erstellen von open-Erweiterungen für Outlook-Ressourcen:

- Erstellen Sie die minimale Anzahl von Erweiterungen erforderlich. Die meisten Clientanwendungen sollten nicht mehr als eine Erweiterung erfordern. Erweiterungen haben keine Eigenschaften festgelegt wird, oder die Struktur, damit Sie mehrere Werte in einer Erweiterung speichern können.
- Benennen Sie Erweiterungen in einer Variablen Weise (z. B. basierend auf Benutzereingaben usw..). Jedes Mal, wenn eine open Erweiterung mit einem neuen Namen erstellt wird, die nicht im Postfach eines Benutzers vor, verwendet wurde, wird ein neues MAPI benannte Eigenschaft erstellt. Entfernen die Erweiterung, die benannte Eigenschaft nicht entfernt.

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>Verwenden Sie open-Erweiterungen (für Outlook-Ressourcen) oder erweiterten Eigenschaften

Open Extensions ist die empfohlene Lösung für die meisten Szenarien im Zusammenhang mit Speichern von und Zugreifen auf benutzerdefinierte Daten. Wenn Sie benutzerdefinierte Daten für Outlook-MAPI-Eigenschaften, die noch nicht verfügbar gemacht werden über die [Microsoft Graph-API-Metadaten](https://developer.microsoft.com/graph/docs/overview/call_api)zugreifen möchten, können Sie [Erweiterte Eigenschaften und der REST-API](extended-properties-overview.md)verwenden. Sie können überprüfen, welche Eigenschaften die Metadaten zur verfügbar gemacht [ https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.opentypeextension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|extensionName|String|Ein eindeutiger Textbezeichner für eine OpenType-Datenerweiterung. Erforderlich. |
|id|String| Eine vollqualifizierte ID, die den Erweiterungstyp mit dem **extensionName**-Element verkettet. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen

Keine

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:---------------|:--------|:----------|
|[Post](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](opentypeextension.md) (in einer vorhandenen Ressource Instanz) oder ein neuer [Kontakt](../resources/contact.md), [Ereignis](../resources/event.md)oder [Nachricht](../resources/message.md) , die ein OpenTypeExtension-Objekt enthält. | Dient zum Erstellen eines openTypeExtension-Objekts in einer vorhandenen oder neuen Ressourceninstanz.|
|[Get](../api/opentypeextension-get.md) | [openTypeExtension](opentypeextension.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des openTypeExtension-Objekts.|
|[Update](../api/opentypeextension-update.md) | [openTypeExtension](opentypeextension.md) |Dient zum Aktualisieren des openTypeExtension-Objekts. |
|[Delete](../api/opentypeextension-delete.md) | Keine |Dient zum Löschen des openTypeExtension-Objekts. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->