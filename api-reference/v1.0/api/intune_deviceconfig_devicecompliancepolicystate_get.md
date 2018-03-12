# <a name="get-devicecompliancepolicystate"></a>deviceCompliancePolicyState abrufen

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Lesen von Eigenschaften und Beziehungen des [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)-Objekts.
## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /managedDevices/{managedDevicesId}/deviceCompliancePolicyStates/{deviceCompliancePolicyStateId}
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.
## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Erforderlich.|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel
### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
GET https://graph.microsoft.com/v1.0/managedDevices/{managedDevicesId}/deviceCompliancePolicyStates/{deviceCompliancePolicyStateId}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1101

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicyState",
    "id": "2999e387-e387-2999-87e3-992987e39929",
    "settingStates": [
      {
        "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState",
        "setting": "Setting value",
        "settingName": "Setting Name value",
        "instanceDisplayName": "Instance Display Name value",
        "state": "notApplicable",
        "errorCode": 9,
        "errorDescription": "Error Description value",
        "userId": "User Id value",
        "userName": "User Name value",
        "userEmail": "User Email value",
        "userPrincipalName": "User Principal Name value",
        "sources": [
          {
            "@odata.type": "microsoft.graph.settingSource",
            "id": "Id value",
            "displayName": "Display Name value"
          }
        ],
        "currentValue": "Current Value value"
      }
    ],
    "displayName": "Display Name value",
    "version": 7,
    "platformType": "iOS",
    "state": "notApplicable",
    "settingCount": 12
  }
}
```



