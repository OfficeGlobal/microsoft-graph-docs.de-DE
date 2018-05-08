# <a name="outlookcategory-resource-type"></a>outlookCategory-Ressourcentyp


Stellt eine Kategorie dar, anhand der ein Benutzer Outlook-Elemente, z. B. Nachrichten und Ereignisse, gruppieren kann. Der Benutzer definiert Kategorien in einer Masterliste und kann eine oder mehrere dieser benutzerdefinierten Kategorien auf ein Element anwenden. 

Mithilfe der REST-API können Sie Kategorien für einen Benutzer in der Masterliste [erstellen](../api/outlookuser_post_mastercategories.md) und definieren. Sie können auch [dieser Masterliste mit Kategorien erhalten](../api/outlookuser_list_mastercategories.md), [eine bestimmte Kategorie abrufen](../api/outlookcategory_get.md), [aktualisieren](../api/outlookcategory_update.md) die Farbe einer Kategorie, oder [Löschen](../api/outlookcategory_delete.md)eine Kategorie. Sie können eine Kategorie auf ein Element anwenden, indem Sie die **displayName**-Eigenschaft der Kategorie der **categories**-Sammlung des Elements zuweisen.
Ressourcen, die Kategorien zugewiesen werden können, sind [contact](contact.md), [event](event.md), [message](message.md) und [post](post.md).   

Jede Kategorie weist zwei Eigenschaften auf: **displayName** und **color**. Der Wert **displayName** muss in der Masterliste eines Benutzers eindeutig sein. Die **color**-Eigenschaft muss jedoch nicht eindeutig sein; mehrere Kategorien in der Masterliste können derselben Farbe zugeordnet werden. Sie können bis zu 25 verschiedene Farben Kategorien in der Masterliste eines Benutzers zuordnen.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|displayName|Zeichenfolge|Ein eindeutiger Name, der eine Kategorie im Postfach des Benutzers identifiziert. Nach der Erstellung einer Kategorie kann der Namen nicht geändert werden. Schreibgeschützt.|
|color|Zeichenfolge|Eine voreingestellte Konstante, die eine Kategorie charakterisiert und einer von 25 vordefinierten Farben zugeordnet ist. Siehe folgenden Hinweis. |

> **Hinweis** Die möglichen Werte für **color** sind vordefinierte Konstanten wie `None`, `preset0` und `preset1`. Jede voreingestellte Konstante ist weiter einer Farbe zugeordnet. Die tatsächliche Farbe ist von dem Outlook-Client abhängig, auf dem die Kategorien angezeigt werden. In der folgenden Tabelle sind die Farben dargestellt, die den einzelnen vordefinierten Konstanten für Outlook (Desktopclient) zugeordnet sind. 


| Voreingestellte Konstante  | In Outlook zugeordnete Farbe |
|:---------------|:--------|
| Keine | Keine Farbe zugeordnet |
| Preset0 | Red |
| Preset1 | Orange |
| Preset2 | Brown |
| Preset3 | Yellow |
| Preset4 | Green |
| Preset5 | Teal |
| Preset6 | Olive |
| Preset7 | Blau |
| Preset8 | Purple |
| Preset9 | Cranberry |
| Preset10 | Steel |
| Preset11 | DarkSteel |
| Preset12 | Gray |
| Preset13 | DarkGray |
| Preset14 | Black |
| Preset15 | DarkRed |
| Preset16 | DarkOrange |
| Preset17 | DarkBrown |
| Preset18 | DarkYellow |
| Preset19 | DarkGreen |
| Preset20 | DarkTeal |
| Preset21 | DarkOlive |
| Preset22 | DarkBlue |
| Preset23 | DarkPurple |
| Preset24 | DarkCranberry |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookCategory"
}-->

```json
{
  "color": "String",
  "displayName": "String"
}

```

## <a name="methods"></a>Methoden
| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Kategorien auflisten](../api/outlookuser_list_mastercategories.md) | [outlookCategory](../resources/outlookcategory.md)-Sammlung |Ruft alle Kategorien ab, die für den Benutzer definiert wurden.|
|[Kategorie abrufen](../api/outlookcategory_get.md) | [outlookCategory](../resources/outlookcategory.md) |Dient zum Abrufen der Eigenschaften und Beziehungen des angegebenen **outlookCategory**-Objekts.|
|[Erstellen](../api/outlookuser_post_mastercategories.md) | [outlookCategory](../resources/outlookcategory.md) |Erstellen eines **outlookCategory**-Objekts in der Masterliste von Kategorien.|
|[Aktualisieren](../api/outlookcategory_update.md) | [outlookCategory](../resources/outlookcategory.md) |Aktualisieren Sie die schreibbare Eigenschaft, **color**, des angegebenen **outlookCategory**-Objekts. |
|[Löschen](../api/outlookcategory_delete.md) | Keine |Löscht das angegebene **outlookCategory**-Objekt. |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
 