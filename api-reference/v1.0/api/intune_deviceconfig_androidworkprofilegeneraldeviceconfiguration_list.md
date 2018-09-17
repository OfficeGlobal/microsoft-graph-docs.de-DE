# <a name="list-androidworkprofilegeneraldeviceconfigurations"></a><span data-ttu-id="2f282-101">Auflisten von androidWorkProfileGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="2f282-101">List androidWorkProfileGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="2f282-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2f282-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f282-103">Eigenschaften und Beziehungen der [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)-Objekte auflisten.</span><span class="sxs-lookup"><span data-stu-id="2f282-103">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f282-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2f282-104">Prerequisites</span></span>
<span data-ttu-id="2f282-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f282-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2f282-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2f282-107">Permission type</span></span>|<span data-ttu-id="2f282-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2f282-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f282-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2f282-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2f282-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f282-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2f282-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2f282-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f282-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f282-112">Not supported.</span></span>|
|<span data-ttu-id="2f282-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2f282-113">Application</span></span>|<span data-ttu-id="2f282-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f282-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f282-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f282-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2f282-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f282-116">Request headers</span></span>
|<span data-ttu-id="2f282-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2f282-117">Header</span></span>|<span data-ttu-id="2f282-118">Wert</span><span class="sxs-lookup"><span data-stu-id="2f282-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f282-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2f282-119">Authorization</span></span>|<span data-ttu-id="2f282-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2f282-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f282-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="2f282-121">Accept</span></span>|<span data-ttu-id="2f282-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="2f282-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f282-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2f282-123">Request body</span></span>
<span data-ttu-id="2f282-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2f282-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f282-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f282-125">Response</span></span>
<span data-ttu-id="2f282-126">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) zurück.</span><span class="sxs-lookup"><span data-stu-id="2f282-126">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f282-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f282-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f282-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f282-128">Request</span></span>
<span data-ttu-id="2f282-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f282-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="2f282-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f282-130">Response</span></span>
<span data-ttu-id="2f282-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f282-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2200

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
      "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "passwordBlockFingerprintUnlock": true,
      "passwordBlockTrustAgents": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "passwordRequiredType": "lowSecurityBiometric",
      "workProfileDataSharingType": "preventAny",
      "workProfileBlockNotificationsWhileDeviceLocked": true,
      "workProfileBlockAddingAccounts": true,
      "workProfileBluetoothEnableContactSharing": true,
      "workProfileBlockScreenCapture": true,
      "workProfileBlockCrossProfileCallerId": true,
      "workProfileBlockCamera": true,
      "workProfileBlockCrossProfileContactsSearch": true,
      "workProfileBlockCrossProfileCopyPaste": true,
      "workProfileDefaultAppPermissionPolicy": "prompt",
      "workProfilePasswordBlockFingerprintUnlock": true,
      "workProfilePasswordBlockTrustAgents": true,
      "workProfilePasswordExpirationDays": 1,
      "workProfilePasswordMinimumLength": 0,
      "workProfilePasswordMinNumericCharacters": 7,
      "workProfilePasswordMinNonLetterCharacters": 9,
      "workProfilePasswordMinLetterCharacters": 6,
      "workProfilePasswordMinLowerCaseCharacters": 9,
      "workProfilePasswordMinUpperCaseCharacters": 9,
      "workProfilePasswordMinSymbolCharacters": 6,
      "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
      "workProfilePasswordPreviousPasswordBlockCount": 13,
      "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
      "workProfilePasswordRequiredType": "lowSecurityBiometric",
      "workProfileRequirePassword": true,
      "securityRequireVerifyApps": true
    }
  ]
}
```








