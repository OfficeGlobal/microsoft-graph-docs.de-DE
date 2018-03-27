# <a name="grouplifecyclepolicy-resource-type"></a>groupLifecyclePolicy-Ressourcentyp

Steht für eine Lebenszyklusrichtlinie für eine Office 365-Gruppe. Eine Lebenszyklusrichtlinie für eine Gruppe ermöglicht Administratoren das Festlegen eines Ablaufzeitraums für Gruppen. Zum Beispiel nach 180 Tagen läuft eine Gruppe ab. Wenn eine Gruppe den Ablaufzeitpunkt erreicht, müssen Besitzer der Gruppe die Gruppe in einem vom Administrator definierten Zeitintervall verlängern. Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der Tage verlängert, die in der Richtlinie definiert sind. Der neue Ablaufzeitraum für die Gruppe lautet dann beispielsweise 180 Tage ab Verlängerung. Wenn die Gruppe nicht verlängert wird, läuft sie ab und wird gelöscht. Die Gruppe kann innerhalb von 30 Tagen nach Löschung wiederhergestellt werden.

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:---------------|:--------|:----------|
|[Get groupLifecyclePolicy](../api/grouplifecyclepolicy_get.md) | [groupLifecyclePolicy](grouplifecyclepolicy.md) |Dient zum Lesen der Eigenschaften und der Beziehungen eines groupLifecyclePolicy-Objekts.|
|[List groupLifecyclePolicies](../api/grouplifecyclepolicy_list.md) | [groupLifecyclePolicy](grouplifecyclepolicy.md)-Sammlung | Listet alle groupLifecyclePolicies auf. |
|[Update groupLifecyclePolicy](../api/grouplifecyclepolicy_update.md) | [groupLifecyclePolicy](grouplifecyclepolicy.md) | Aktualisiert ein groupLifecyclePolicy-Objekt. |
|[Delete groupLifecyclePolicy](../api/grouplifecyclepolicy_delete.md) | Keine | Löscht ein groupLifecyclePolicy-Objekt. |
|[Add a group to a groupLifecyclePolicy](../api/grouplifecyclepolicy_addgroup.md)|Keine| Fügt eine Gruppe zu einer Lebenszyklusrichtlinie hinzu. |
|[Remove a group from a groupLifecyclePolicy](../api/grouplifecyclepolicy_removegroup.md)|Keine| Entfernt eine Gruppe aus einer Lebenszyklusrichtlinie. |

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|alternateNotificationEmails|Zeichenfolge| Liste der E-Mail-Adressen, an die Benachrichtigungen für Gruppen ohne Besitzer gesendet werden sollen. Mehrere E-Mail-Adressen können durch ein Semikolon voneinander getrennt definiert werden. |
|groupLifetimeInDays|Int32| Anzahl von Tagen, bis eine Gruppe abläuft und verlängert werden muss. Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der definierten Tage verlängert. |
|id|Guid| Ein eindeutiger Bezeichner für eine Richtlinie. Schreibgeschützt.|
|managedGroupTypes|Zeichenfolge| Der Gruppentyp, für den die Ablaufrichtlinie gilt. Mögliche Werte sind **Alle**, **Ausgewählte** oder **Keine**. |

## <a name="relationships"></a>Beziehungen

Keine.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
}-->

```json
{
  "alternateNotificationEmails": "String",
  "groupLifetimeInDays": 180,
  "id": "Guid (identifier)",
  "managedGroupTypes": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->