# <a name="create-deviceenrollmentlimitconfiguration"></a>deviceEnrollmentLimitConfiguration erstellen

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Erstellen eines neuen [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md)-Objekts.
## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das deviceEnrollmentLimitConfiguration-Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceEnrollmentLimitConfiguration erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)|
|displayName|String|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)|
|description|String|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)|
|Priorität|Int32|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)|
|Version|Int32|Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)|
|Begrenzung|Int32|Noch nicht dokumentiert.|



## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel
### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 269

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 377

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```


