# <a name="directoryrole-resource-type"></a>Ressourcentyp directoryRole

Stellt eine Azure AD-Verzeichnisrolle dar. Azure AD-Verzeichnisrollen werden auch als *Administratorrollen* bezeichnet. Weitere Informationen zu diesen Verzeichnis-(Administrator)Rollen finden Sie unter [Zuweisen von Administratorrollen in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). Mit Microsoft Graph können Sie Benutzer zu Verzeichnisrollen zuweisen, um ihnen Berechtigungen der Zielrolle zuzuweisen. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren sind standardmäßig aktiviert. Zum Aktivieren anderer verfügbarer Verzeichnisrollen senden Sie eine POST-Anforderung mit der ID der [directoryRoleTemplate](directoryroletemplate.md), auf der die Verzeichnisrolle basiert. Erbt von [directoryObject](directoryobject.md).



## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[directoryRole abrufen](../api/directoryrole_get.md) | [directoryRole](directoryrole.md) | Dient zum Lesen der Eigenschaften und der Beziehungen des directoryRole-Objekts. |
|[Mitglied erstellen](../api/directoryrole_post_members.md) |[directoryObject](directoryobject.md)| Fügen Sie der Verzeichnisrolle einen Benutzer durch Veröffentlichen in der Mitgliedernavitionseingenschaft hinzu.|
|[Mitglieder auflisten](../api/directoryrole_list_members.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Benutzer, die Mitglieder der Verzeichnisrolle sind, aus der Mitgliedernavigationseigenschaft ab.|
|[Mitglied entfernen](../api/directoryrole_delete_member.md) |[directoryObject](directoryobject.md)| Dient zum Entfernen eines Benutzers aus der Verzeichnisrolle.|
|[directoryRole aktivieren](../api/directoryrole_post_directoryroles.md) |[directoryRole](directoryrole.md) | Dient zum Aktivieren einer Verzeichnisrolle.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft   | Typ | Beschreibung |
|:---------------|:--------|:----------|
|description|String|Die Beschreibung für die Verzeichnisrolle. Schreibgeschützt. |
|displayName|String|Der Anzeigename für die Verzeichnisrolle. Schreibgeschützt. |
|id|String|Die eindeutige ID für die Verzeichnisrolle. Geerbt von [directoryObject](directoryobject.md). Schlüssel, lässt keine Nullwerte zu, schreibgeschützt.|
|roleTemplateId|String| Die **id** der [directoryRoleTemplate](directoryroletemplate.md), auf der diese Rolle basiert. Die Eigenschaft muss angegeben werden, wenn eine Verzeichnisrolle mit einer POST-Operation in einem Mandanten aktiviert wird. Nach der Aktivierung der Verzeichnisrolle ist die Eigenschaft schreibgeschützt. |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ |Beschreibung|
|:---------------|:--------|:----------|
|Elemente|[directoryObject](directoryobject.md)-Sammlung|Benutzer, die Mitglieder dieser Verzeichnisrolle sind. HTTP-Methoden: GET, POST, DELETE. Schreibgeschützt. Lässt Nullwerte zu.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRole"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "roleTemplateId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
