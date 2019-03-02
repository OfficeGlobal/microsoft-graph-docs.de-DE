---
title: companyInformation-Ressourcentyp
description: Unternehmensinformationen in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0f8671cbade11cc9db6bf797c39eb17acf286ef7
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365913"
---
# <a name="companyinformation-resource-type"></a>companyInformation-Ressourcentyp
Stellt die für das aktuelle Unternehmen in Dynamics 365 Business Central angegebenen Informationen wie Name, Adresse, e-Mail-Adresse und Websiteadresse dar.

## <a name="methods"></a>Methoden

| Methode         | Rückgabetyp  |Beschreibung|
|:---------------|:-------------|:----------|
|[CompanyInformation abrufen](../api/dynamics-companyinformation-get.md)|companyInformation|Ruft Unternehmensinformationen ab.|
|[Patch-companyInformation](../api/dynamics-companyinformation-update.md)|companyInformation|Aktualisiert Unternehmensinformationen.|


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ      |Beschreibung                           |
|:-------------|:--------|:-------------------------------------|
|id            |GUID|Die eindeutige ID des Unternehmens. Nicht bearbeitbar.|
|displayName   |string   |Der Anzeigename des Unternehmens.           |
|address       |[Navigations. PostalAddress](../resources/dynamics-complextypes.md)|Die Adresse des Unternehmens. Zeigen Sie den komplexen Typ für zusätzliche Details an.|
|PhoneNumber   |string   |Die Telefonnummer des Unternehmens.       |
|faxNumber     |string   |Die Faxnummer des Unternehmens.             |
|email         |string   |Die e-Mail-Adresse des Unternehmens.          |
|Website       |string   |Die Websiteadresse des Unternehmens.        |
|taxRegistrationNumber|string|Die Steuernummer des Unternehmens.|
|currencyCode  |string   |Die Währung, in der das Unternehmen tätig ist. Schreibgeschützt.|
|currentFiscalYearStartDate|date|Das aktuelle Geschäftsjahr-Anfangsdatum des Unternehmens. Schreibgeschützt.|
|Industrie      |string   |Die Branche, zu der das Unternehmen gehört.  |
|Bild       |stream   |Das Firmen Logo. Schreibgeschützt.          |
|businessProfileId|string|Die Geschäftsprofil-ID, die mit dem Financials-Unternehmen verknüpft ist. Schreibgeschützt.|
|lastModifiedDateTime|DateTime|Die letzte Uhrzeit, zu der das Unternehmen geändert wurde. Schreibgeschützt.|  


## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung des companyInformation
```json
{
  "id": "GUID",
  "displayName": "string",
  "address": "NAV.PostalAddress",
  "phoneNumber": "string",
  "faxNumber": "string",
  "email": "string",
  "website": "string",
  "taxRegistrationNumber": "string",
  "currencyCode": "string",
  "currentFiscalYearStartDate": "date",
  "industry": "string",
  "picture": "stream",
  "businessProfileId": "string",
  "lastModifiedDateTime": "datetime"
}

```

