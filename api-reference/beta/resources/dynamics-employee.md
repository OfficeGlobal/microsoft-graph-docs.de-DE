---
title: Employees-Ressourcentyp
description: Ein Employee-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 865da0c1e1256e2ba2a25902e37a00da9081eedf
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366655"
---
# <a name="employees-resource-type"></a>Employees-Ressourcentyp
Stellt einen Mitarbeiter in Dynamics 365 Business Central dar.

## <a name="methods"></a>Methoden

| Methode                                              | Rückgabetyp|Beschreibung               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[Mitarbeiter abrufen](../api/dynamics-employee-get.md)      |Mitarbeiter  |Rufen Sie ein Employee-Objekt ab.   |
|[Post Angestellte](../api/dynamics-create-employee.md)  |Mitarbeiter  |Erstellen eines Employee-Objekts.|
|[Patch-Mitarbeiter](../api/dynamics-employee-update.md) |Mitarbeiter  |Aktualisieren eines Employee-Objekts.|
|[Mitarbeiter löschen](../api/dynamics-employee-delete.md)|Keine       |Löschen eines Employee-Objekts.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft           | Typ   |Beschreibung                                            |
|:-------------------|:-------|:------------------------------------------------------|
|id                  |GUID    |Die Mitarbeiter-ID. Nicht bearbeitbar.                         |
|number              |string  |Die Mitarbeiternummer. Schreibgeschützt.                        |
|displayName         |String  |Der angegebene Name und Nachname des Mitarbeiters. Schreibgeschützt.           |
|givenName           |string  |Der angegebene Name des Mitarbeiters.                        |
|middleName          |string  |Der Vorname des Mitarbeiters.                       |
|surname             |string  |Der Nachname des Mitarbeiters                            |
|jobTitle            |string  |Der vollständige Name des Mitarbeiters                          |
|address             |[Navigations. PostalAddress](../resources/dynamics-complextypes.md)|Gibt die Adresse des Mitarbeiters an. Diese Adresse wird in allen Ressourcen Dokumenten des Mitarbeiters angezeigt.|
|PhoneNumber         |string  |Gibt die Telefonnummer des Mitarbeiters an.             |
|mobilePhone         |string  |Gibt die Mobiltelefonnummer des Mitarbeiters an.      |
|email               |string  |Gibt die e-Mail-Adresse des Mitarbeiters an.                |
|personalEmail       |string  |Gibt die persönliche e-Mail-Adresse des Mitarbeiters an.       |
|employmentDate      |date    |Gibt das Datum an, an dem der Mitarbeiter begonnen hat, für das Unternehmen zu arbeiten.|
|terminationDate     |date    |Gibt das Datum an, an dem der Mitarbeiter beendet wurde, beispielsweise aufgrund eines Ausfalls oder einer Kündigung.|
|status              |string  |Gibt den Status des Mitarbeiters an. Mögliche Werte sind aktiv, inaktiv oder terminiert|
|birthDate           |date    |Gibt das Geburtsdatum des Mitarbeiters an.                |
|Bild             |stream  |Das Bild des Mitarbeiters. Schreibgeschützt.                       |
|lastModifiedDateTime|DateTime|Die letzte DateTime, die der Mitarbeiter geändert wurde. Schreibgeschützt.|  


## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.


```json
{
    "id": "GUID",
    "number": "string",
    "displayName": "string",
    "givenName": "string",
    "middleName": "string",
    "surname": "string",
    "jobTitle": "string",
    "address": "NAV.PostalAddress",
    "phoneNumber": "string",
    "mobilePhone": "string",
    "email": "string",
    "personalEmail": "string",
    "employmentDate": "date",
    "terminationDate": "date",
    "status": "string",
    "birthDate": "date",
    "picture": "stream",
    "lastModifiedDateTime": "datetime"
}

```

