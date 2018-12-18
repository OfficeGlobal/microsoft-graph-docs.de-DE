---
title: Aktualisieren von „deviceAppManagement“
description: Aktualisiert die Eigenschaften von Objekten des Typs deviceAppManagement.
author: tfitzmac
ms.openlocfilehash: d5a4b3cfa1af7eb4a465c951a4a10f4c19944d8a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324024"
---
# <a name="update-deviceappmanagement"></a>Aktualisieren von „deviceAppManagement“

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Aktualisiert die Eigenschaften von Objekten des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).
## <a name="prerequisites"></a>Voraussetzungen
Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).  Beachten Sie, dass die entsprechende Berechtigungen gemäß den Workflow variiert.

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
| Delegiert (Geschäfts-, Schul- oder Unikonto) | |
| &nbsp;&nbsp; **Apps**, **Bücher**oder **Onboarding** | DeviceManagementApps.ReadWrite.All |
| &nbsp; &nbsp; **Geräteverwaltung** | DeviceManagementManagedDevices.ReadWrite.All |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
| Anwendung | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a>Anforderungsheader
|Header|Wert|
|:---|:---|
|Autorisierung|Bearer&lt;token&gt; erforderlich|
|Accept|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) an.

In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|**Klicken Sie auf mittels Fingereingabe**|
|isEnabledForMicrosoftStoreForBusiness|Boolescher Wert|Gibt an, ob das Konto Anwendungen mit dem Microsoft Store für Unternehmen synchronisieren darf.|
|microsoftStoreForBusinessLanguage|String|Die Gebietsschemainformationen, die zur Synchronisierung von Anwendungen mit dem Microsoft Store für Unternehmen verwendet werden. Angegeben werden Kulturen, die für ein Land bzw. eine Region spezifisch sind. Die Namen dieser Kulturen folgen dem Standard RFC 4646 (Windows Vista und höher). Das Format lautet <languagecode2>-<country/regioncode2>. Dabei ist <languagecode2> ein klein geschriebener Code aus zwei Buchstaben nach ISO 639-1 und <country/regioncode2> ein groß geschriebener Code aus zwei Buchstaben nach ISO 3166. Beispiel für eine spezifische Kultur: „en-US“ für „Englisch (Vereinigte Staaten)“.|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|Zeitpunkt der letzten Anwendungssynchronisierung mit dem Microsoft Store für Unternehmen|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|Zeitpunkt, zu dem das Konto die Apps letztmals erfolgreich mit dem Microsoft Store für Unternehmen synchronisiert hat|
|microsoftStoreForBusinessPortalSelection|[microsoftStoreForBusinessPortalSelectionOptions](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|Die Endbenutzer Portal-Informationen werden verwendet, aus dem Microsoft Store for Business Applications, Intune Unternehmen Portal synchronisieren. Es gibt drei Optionen zur Auswahl \['Des Unternehmens nur Portal', 'Unternehmen Portal und privaten speichern', 'Privaten Speicher'\]. Mögliche Werte sind: `none`, `companyPortal` und `privateStore`.|

Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.

## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.

``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



