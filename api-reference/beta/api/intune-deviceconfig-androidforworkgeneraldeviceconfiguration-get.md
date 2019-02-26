---
title: AndroidForWorkGeneralDeviceConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des androidForWorkGeneralDeviceConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76896c963f91a362d3b81734fc1f3aa07bcbe2bd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157652"
---
# <a name="get-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="71c87-103">AndroidForWorkGeneralDeviceConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="71c87-103">Get androidForWorkGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="71c87-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="71c87-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71c87-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="71c87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71c87-106">Lesen von Eigenschaften und Beziehungen des [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="71c87-106">Read properties and relationships of the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71c87-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="71c87-107">Prerequisites</span></span>
<span data-ttu-id="71c87-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="71c87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="71c87-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="71c87-110">Permission type</span></span>|<span data-ttu-id="71c87-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="71c87-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71c87-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="71c87-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71c87-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="71c87-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="71c87-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="71c87-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71c87-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71c87-115">Not supported.</span></span>|
|<span data-ttu-id="71c87-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="71c87-116">Application</span></span>|<span data-ttu-id="71c87-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71c87-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71c87-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71c87-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71c87-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="71c87-119">Optional query parameters</span></span>
<span data-ttu-id="71c87-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="71c87-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71c87-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="71c87-121">Request headers</span></span>
|<span data-ttu-id="71c87-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="71c87-122">Header</span></span>|<span data-ttu-id="71c87-123">Wert</span><span class="sxs-lookup"><span data-stu-id="71c87-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71c87-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="71c87-124">Authorization</span></span>|<span data-ttu-id="71c87-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="71c87-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71c87-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="71c87-126">Accept</span></span>|<span data-ttu-id="71c87-127">application/json</span><span class="sxs-lookup"><span data-stu-id="71c87-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71c87-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="71c87-128">Request body</span></span>
<span data-ttu-id="71c87-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="71c87-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71c87-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="71c87-130">Response</span></span>
<span data-ttu-id="71c87-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="71c87-131">If successful, this method returns a `200 OK` response code and [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71c87-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71c87-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="71c87-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71c87-133">Request</span></span>
<span data-ttu-id="71c87-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="71c87-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="71c87-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="71c87-135">Response</span></span>
<span data-ttu-id="71c87-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71c87-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2323

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
    "id": "a931a366-a366-a931-66a3-31a966a331a9",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
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
    "securityRequireVerifyApps": true,
    "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
    "vpnEnableAlwaysOnLockdownMode": true
  }
}
```




