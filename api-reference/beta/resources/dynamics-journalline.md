---
title: journalLines-Ressourcentyp
description: Eine Journal Zeile in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 7a6841bcc2f893f8ca794e7d8e6aeafbcd4e48ca
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365955"
---
# <a name="journallines-resource-type"></a>journalLines-Ressourcentyp
Stellt eine Zeile in einem Journal in Dynamics 365 Business Central dar.

## <a name="methods"></a>Methoden

| Methode                                                    | Rückgabetyp|Beschreibung         |
|:----------------------------------------------------------|:-----------|:-------------------|
|[JournalLines abrufen](../api/dynamics-journalline-get.md)      |journalLines|Ruft eine Journal Zeile ab.   |
|[Post journalLines](../api/dynamics-create-journalline.md)  |journalLines|Erstellt eine Journal Zeile.|
|[Patch-journalLines](../api/dynamics-journalline-update.md) |journalLines|Aktualisiert eine Journal Zeile.|
|[JournalLines löschen](../api/dynamics-journalline-delete.md)|Keine        |Löscht eine Journal Zeile.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft             | Typ                   |Beschreibung                                                        |
|:---------------------|:-----------------------|:------------------------------------------------------------------|
|id                    |GUID                    |Die eindeutige ID der Erf.-Journal Zeile. Nicht bearbeitbar.                   |
|journalDisplayName    |Zeichenfolge, maximale Größe 10 |Der Anzeigename des Journals, zu dem diese Zeile gehört. Schreibgeschützt.|
|lineNumber            |integer                 |Die Nummer der Erf.-Journal Zeile.                                    |
|accountId             |GUID                    |Die eindeutige ID des Kontos, mit dem die Journal Zeile verknüpft ist.  |
|accountNumber         |Zeichenfolge, maximale Größe 20 |Die Nummer des Kontos, mit dem die Erf.-Journal Zeile verknüpft ist.     |
|postingDate           |date                    |Das Datum, an dem die Erf.-Journal Zeile gebucht wurde.                          |
|documentNumber        |Zeichenfolge, maximale Größe 20 |Gibt eine Dokumentnummer für die Erf.-Journal Zeile an.                  |
|externalDocumentNumber|Zeichenfolge, maximale Größe 20 |Gibt eine externe Dokumentnummer für die Erf.-Journal Zeile an.        |
|Menge                |decimal                 |Gibt den Gesamtbetrag (einschließlich MwSt.) an, aus dem die Erf.-Journal Zeile besteht.|
|description           |Zeichenfolge, maximale Größe 50 |Die Beschreibung der Erf.-Journal Zeile, die vom Benutzer bereitgestellt oder selbst erstellt wurde.|
|Kommentar               |Zeichenfolge, maximale Größe 250|Ein benutzerdefinierter Kommentar in der Erf.-Journal Zeile.                      |
|lastModifiedDateTime  |DateTime                |Die letzte Uhrzeit, zu der die Journal Zeile geändert wurde. Schreibgeschützt.        |

## <a name="relationships"></a>Beziehungen
Eine Buch.-Blattzeile ist eine Unterseite eines Journals. Er kann nicht direkt zugegriffen werden.

Eine Buch.-Blattzeile kann eine "übergeordnete Entität" der Maßlinie sein.

In der Tabelle Konten muss ein Konto (Konto-Nr.) vorhanden sein.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.


```json
{
    "id": "GUID",
    "journalDisplayName": "string",
    "lineNumber": "integer",
    "accountId": "GUID",
    "accountNumber": "string",
    "postingDate": "date",
    "documentNumber": "string",
    "externalDocumentNumber": "string",
    "amount": "decimal",
    "description": "string",
    "comment": "string",
    "lastModifiedDateTime": "datetime"
}
```
