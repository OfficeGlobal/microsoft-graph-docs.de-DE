# <a name="opentypeextension-resource-type-open-extensions"></a>openTypeExtension-Ressourcentyp (offene Erweiterungen)

Offene Erweiterungen (bisher als Office 365-Datenerweiterungen bezeichnet) bieten Ihnen eine einfache Möglichkeit zum direkten Hinzufügen nicht typisierter Eigenschaften zu einer Ressource in Microsoft Graph. Offiene Erweiterungen werden mithilfe der **openTypeExtension**-Ressource dargestellt. Alle offenen Erweiterungen, die einer Ressource hinzugefügt wurden, werden in der **extensions**-Navigationseigenschaft angezeigt, die vom abstrakten Typ [extension](extension.md) abgeleitet wird.  Jede Erweiterung weist eine **extensionName**-Eigenschaft auf, die die einzige vordefinierte, schreibbare Eigenschaft für alle Erweiterungen zusammen mit ihren benutzerdefinierten Daten ist. Um sicherzustellen, dass Erweiterungsnamen eindeutig sind, können Sie eine umgekehrtes DNS-Format (Domain Name System) verwenden, das _von Ihrer eigenen Domäne_, z. B. `Com.Contoso.ContactInfo`, abhängig ist. Verwenden Sie in Erweiterungsnamen auf keinen Fall die Microsoft-Domäne (`Com.Microsoft` oder `Com.OnMicrosoft`).

Beispiel für eine offene Erweiterung: [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](../../../concepts/extensibility_open_users.md)

Offene Erweiterungen werden von den folgenden Ressourcen in den entsprechenden Versionen unterstützt: - Allgemein verfügbar (GA: /v1.0 und /beta) oder Vorschau (/beta).

| Ressource | Version |
|---------------|-------|
| [Administrative Einheit](../../beta/resources/administrativeunit.md)  | Nur Vorschau |
| [Kalenderereignis](event.md) | Allgemein verfügbar |
| [Kalenderereignis](event.md) für Gruppe | Allgemein verfügbar |
| Unterhaltungsthread der Gruppe [posten](post.md) | Allgemein verfügbar |
| [device](device.md) | Allgemein verfügbar |
| [group](group.md) | Allgemein verfügbar |
| [message](message.md) | Allgemein verfügbar |
| [organization](organization.md) | Allgemein verfügbar |
| [Personal contact](contact.md) | Allgemein verfügbar |
| [user](user.md) | Allgemein verfügbar |


### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>Sollen offene Erweiterungen (für Outlook-Ressourcen) oder erweiterte Eigenschaften verwendet werden?

Offene Erweiterungen sind die empfohlene Lösung für die meisten Szenarios, bei denen benutzerdefinierte Daten gespeichert und aufgerufen werden sollen. Wenn Sie auf benutzerdefinierte Daten für Outlook-MAPI-Eigenschaften zugreifen müssen, die nicht bereits in den [Microsoft Graph-API-Metadaten](http://developer.microsoft.com/en-us/graph/docs/overview/call_api) verfügbar gemacht wurden, können Sie [erweiterte Eigenschaften und deren REST-API](extended-properties-overview.md) verwenden. Unter https://graph.microsoft.com/v1.0/$metadata können Sie überprüfen, welche Eigenschaften die Metadaten verfügbar machen.


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
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|extensionName|Zeichenfolge|Ein eindeutiger Textbezeichner für eine offene Erweiterung. Erforderlich.|
|id|String| Eine vollqualifizierte ID, die den Erweiterungstyp mit dem **extensionName**-Element verkettet. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Post](../api/opentypeextension_post_opentypeextension.md) | [openTypeExtension](opentypeextension.md) (in einer vorhandenen Ressourceninstanz) oder ein neues [contact](../resources/contact.md)-, [event](../resources/event.md)- oder [message](../resources/message.md)-Objekt, das ein openTypeExtension-Objekt enthält. | Dient zum Erstellen eines openTypeExtension-Objekts in einer vorhandenen oder neuen Ressourceninstanz.| 
|[Get](../api/opentypeextension_get.md) | [openTypeExtension](opentypeextension.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des openTypeExtension-Objekts.|
|[Update](../api/opentypeextension_update.md) | [openTypeExtension](opentypeextension.md)    |Dient zum Aktualisieren des openTypeExtension-Objekts. |
|[Delete](../api/opentypeextension_delete.md) | Keine |Dient zum Löschen des openTypeExtension-Objekts. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->