---
title: komplexe Typen JSON
description: Komplexe Datentypen in JSON für Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4fc4d4f53014f5b8c656cd069cadf7b19190e0f0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366767"
---
# <a name="complex-types-json"></a>komplexe Typen JSON
Dies sind die verschiedenen komplexen Typen in Dynamics 365 Business Central. Sie können die Verwendung dieser komplexen Typen in den verschiedenen einzelnen Methoden anzeigen, die Sie verwenden.

## <a name="postal-address"></a>Postanschrift

Stellt einen komplexen Postanschrift-Typ in Dynamics 365 Business Central dar.

### <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ       |Beschreibung             |
|:-------------|:---------|:-----------------------|
|street        |string    |Postanschrift Straße.  |
|city          |string    |Postanschrift Stadt.    |
|state         |string    |Postanschrift.   |
|countryLetterCode|string |Postanschrift Land Buchstabencode (zwei Zeichen Wort)|
|postalCode    |string    |Postanschrift PLZ|

```json
"PostalAddress" 
{ 
"street": "string",
"city": "string", 
"state": "string", 
"countryLetterCode": "string", 
"postalCode": "string" 
} 
 ```

