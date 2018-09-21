# <a name="get-outlook-contacts-in-a-shared-folder"></a>Abrufen von Outlook-Kontakten in einem freigegebenen Ordner

Mit Outlook können Benutzer Ordner freigeben und den Zugriff auf einzelne Kontaktordner "lesen", "erstellen", "ändern" oder "löschen" aktivieren. Outlook ermöglicht es einem Kunden auch, einen anderen Benutzer zu delegieren, um im Auftrag des Kunden zu handeln und auf bestimmte Ordner oder das gesamte Postfach des Kunden zuzugreifen. Dies wird in Outlook auch als "Delegierung" bezeichnet.

Programmgesteuert unterstützt Microsoft Graph das Abrufen von Kontakten in Kontaktordnern, die von anderen Benutzern freigegeben wurden, sowie das Abrufen der freigegebenen Ordner selbst. Der Support gilt auch für Ordner in einem delegierten Postfach.

Als Beispiel hat Garth mit John einen benutzerdefinierten Kontaktordner geteilt und John Lesezugriff gewährt. Wenn John sich in Ihrer App angemeldet und delegierte Berechtigungen (Contacts.Read.Shared oder Contacts.ReadWrite.Shared) bereitgestellt hat, kann Ihre App auf den benutzerdefinierten Kontaktordner und die Kontakte von Garth in diesem Ordner zugreifen, wie nachfolgend beschrieben.

## <a name="get-a-contact-in-the-shared-folder"></a>Abrufen eines Kontakts in den freigegebenen Ordner

Sie können einen bestimmten Kontakt in dem benutzerdefinierten Kontaktordner abrufen, den Garth mit John geteilt hat:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

Nach erfolgreichem Abschluss erhalten Sie HTTP 200 OK und die [ Kontakt](../api-reference/v1.0/resources/contact.md) -Instanz, die von`{id}`   aus dem gemeinsamen Kontaktordner von Garth identifiziert wurde.

## <a name="get-all-contacts-in-the-shared-folder"></a>Abrufen aller Kontakte in dem freigegebenen Ordner

Abrufen aller Kontakte in Garths freigegebenem Kontaktordner:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

Nach erfolgreichem Abschluss erhalten Sie HTTP 200 OK und eine Sammlung von [Kontakt](../api-reference/v1.0/resources/contact.md) Instanzen im gemeinsamen Kontaktordner von Garth.

## <a name="get-the-shared-folder"></a>Abrufen des freigegebenen Ordners

Abrufen des Kontaktordners, den Garth mit John geteilt hat.

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

Nach erfolgreichem Abschluss erhalten Sie HTTP 200 OK und eine [contactFolder](../api-reference/v1.0/resources/contactfolder.md) Instanz, die Garths gemeinsamen Kontaktordner darstellt.

Die gleichen GET-Fähigkeiten gelten, wenn Garth John sein gesamtes Postfach übertragen hat.

Wenn Garth den Kontaktordner nicht mit John geteilt hat oder sein Postfach an John übertragen hat, gibt die Angabe der Benutzer-ID oder des Benutzernamens von Garth in diesen GET-Operationen einen Fehler zurück. 


## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen:

- [Warum persönliche Kontakte in Outlook integrieren?](outlook-contacts-concept-overview.md)
- Die [Kontakte API](../api-reference/v1.0/resources/contact.md) in Microsoft Graph v1. 0.