# <a name="datetimetimezone-resource-type"></a>Ressourcentyp dateTimeTimeZone

Beschreibt das Datum, die Uhrzeit und Zeitzone eines Zeitpunkts.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|DateTime|String|Ein bestimmter Zeitpunkt in einer kombinierten Datums- und Uhrzeitsdarstellung (`<date>T<time>`).|
|TimeZone|String|Einer der folgenden Zeitzonennamen.|

Die Eigenschaft _TimeZone_ kann auf eine beliebige, von Windows unterstützte Zeitzone und auf einen der folgenden Zeitzonennamen eingestellt werden .

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
<!-- {
  "type": "#page.annotation",
  "description": "dateTimeTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
