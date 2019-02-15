---
title: Ressourcentyp dateTimeTimeZone
description: Beschreibt das Datum, die Uhrzeit und Zeitzone eines Zeitpunkts.
localization_priority: Normal
ms.openlocfilehash: ee5359c0ababad2a4f785d17a02ac5bb618d2681
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057043"
---
# <a name="datetimetimezone-resource-type"></a>Ressourcentyp dateTimeTimeZone

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Beschreibt das Datum, die Uhrzeit und Zeitzone eines Zeitpunkts.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|dateTime|String|Ein bestimmter Zeitpunkt in einer kombinierten Datums- und Uhrzeitsdarstellung (`{date}T{time}`). Beispielsweise "2019-04-16T09:00:00".|
|timeZone|Zeichenfolge|Ein Zeitzonenname, wie unten beschrieben.|

Die **TimeZone** -Eigenschaft kann auf eine der von Windows unterstützten Zeitzonen sowie die folgenden Zeitzonen-Namen festgelegt werden.

Etc/GMT+12

Etc/GMT+11

Pazifik/Honolulu

Amerika/Anchorage

Amerika/Santa_Isabel

Amerika/Los_Angeles

Amerika/Phoenix

Amerika/Chihuahua

Amerika/Denver

Amerika/Guatemala

Amerika/Chicago

Amerika/Mexico_Stadt

Amerika/Regina

Amerika/Bogota

Amerika/New_York

Amerika/Indiana/Indianapolis

Amerika/Caracas

Amerika/Asuncion

Amerika/Halifax

Amerika/Cuiaba

Amerika/La_Paz

Amerika/Santiago

Amerika/St_Johns

Amerika/Sao_Paulo

Amerika/Argentinien/Buenos_Aires

Amerika/Cayenne

Amerika/Godthab

Amerika/Montevideo

Amerika/Bahia

Etc/GMT+2

Atlantik/Azoren

Atlantik/Kap_Verde

Afrika/Casablanca

Etc/GMT

Europa/London

Atlantik/Reykjavik

Europa/Berlin

Europa/Budapest

Europa/Paris

Europa/Warschau

Afrika/Lagos

Afrika/Windhoek

Europa/Bukarest

Asien/Beirut

Afrika/Kairo

Asien/Damaskus

Afrika/Johannesburg

Europa/Kiew

Europa/Istanbul

Asien/Jerusalem

Asien/Amman

Asien/Bagdad

Europa/Kaliningrad

Asien/Riad

Afrika/Nairobi

Asien/Teheran

Asien/Dubai

Asien/Baku

Europa/Moskau

Indisch/Mauritius

Asien/Tiflis

Asien/Eriwan

Asien/Kabul

Asien/Karatschi

Asien/Taschkent

Asien/Kolkata

Asien/Colombo

Asien/Katmandu

Asien/Astana (Almaty)

Asien/Dhaka

Asien/Jekaterinburg

Asien/Yangon (Rangun)

Asien/Bangkok

Asien/Nowosibirsk

Asien/Shanghai

Asien/Krasnojarsk

Asien/Singapur

Australien/Perth

Asien/Taipeh

Asien/Ulan-Bator

Asien/Irkutsk

Asien/Tokio

Asien/Seoul

Australien/Adelaide

Australien/Darwin

Australien/Brisbane

Australien/Sydney

Pazifik/Port_Moresby

Australien/Hobart

Asien/Jakutsk

Pazifik/Guadalcanal

Asien/Wladiwostok

Pazifik/Auckland

Etc/GMT-12

Pazifik/Fidschi

Asien/Magadan

Pazifik/Tongatapu

Pazifik/Apia

Pazifik/Kiritimati

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dateTimeTimeZone"
}-->

```json
{
  "dateTime": "string",
  "timeZone": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "dateTimeTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/datetimetimezone.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
