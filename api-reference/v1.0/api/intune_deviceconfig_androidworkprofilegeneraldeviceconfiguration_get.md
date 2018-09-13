# <a name="get-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="9b73e-101">Abrufen von androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="9b73e-101">Get androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="9b73e-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9b73e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b73e-103">Lesen Sie Eigenschaften und Beziehungen des [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9b73e-103">Read properties and relationships of the [deviceAppManagement](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9b73e-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9b73e-104">Prerequisites</span></span>
<span data-ttu-id="9b73e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9b73e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9b73e-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9b73e-107">Permission type</span></span>|<span data-ttu-id="9b73e-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9b73e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b73e-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9b73e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9b73e-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b73e-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9b73e-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9b73e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b73e-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9b73e-112">Not supported.</span></span>|
|<span data-ttu-id="9b73e-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9b73e-113">Application</span></span>|<span data-ttu-id="9b73e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9b73e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b73e-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b73e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9b73e-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9b73e-116">Optional query parameters</span></span>
<span data-ttu-id="9b73e-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9b73e-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9b73e-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9b73e-118">Request headers</span></span>
|<span data-ttu-id="9b73e-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9b73e-119">Header</span></span>|<span data-ttu-id="9b73e-120">Wert</span><span class="sxs-lookup"><span data-stu-id="9b73e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b73e-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9b73e-121">Authorization</span></span>|<span data-ttu-id="9b73e-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9b73e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b73e-123">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="9b73e-123">Accept</span></span>|<span data-ttu-id="9b73e-124">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="9b73e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b73e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9b73e-125">Request body</span></span>
<span data-ttu-id="9b73e-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9b73e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b73e-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b73e-127">Response</span></span>
<span data-ttu-id="9b73e-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen`200 OK`Antwortcode und[androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)-Objekt im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9b73e-128">If successful, this method returns a `200 OK` response code and a [mobileThreatDefenseConnector](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b73e-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9b73e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="9b73e-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b73e-130">Request</span></span>
<span data-ttu-id="9b73e-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9b73e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="9b73e-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b73e-132">Response</span></span>
<span data-ttu-id="9b73e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9b73e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2104

{
  "value": {
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
}
```








