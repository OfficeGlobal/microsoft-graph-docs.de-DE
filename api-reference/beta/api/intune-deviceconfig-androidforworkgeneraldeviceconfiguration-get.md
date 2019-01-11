---
title: Abrufen von androidForWorkGeneralDeviceConfiguration
description: Lesen Sie Eigenschaften und Beziehungen des AndroidForWorkGeneralDeviceConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a926ffdd3954d5a3d56626103b22a319f54e7c61
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817332"
---
# <a name="get-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="9fae7-103">Abrufen von androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="9fae7-103">Get androidForWorkGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="9fae7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9fae7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9fae7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9fae7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9fae7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9fae7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9fae7-107">Lesen Sie Eigenschaften und Beziehungen des [AndroidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9fae7-107">Read properties and relationships of the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9fae7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9fae7-108">Prerequisites</span></span>
<span data-ttu-id="9fae7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fae7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fae7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9fae7-111">Permission type</span></span>|<span data-ttu-id="9fae7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9fae7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fae7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9fae7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9fae7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fae7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9fae7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9fae7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fae7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9fae7-116">Not supported.</span></span>|
|<span data-ttu-id="9fae7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9fae7-117">Application</span></span>|<span data-ttu-id="9fae7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9fae7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fae7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9fae7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9fae7-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9fae7-120">Optional query parameters</span></span>
<span data-ttu-id="9fae7-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9fae7-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9fae7-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9fae7-122">Request headers</span></span>
|<span data-ttu-id="9fae7-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9fae7-123">Header</span></span>|<span data-ttu-id="9fae7-124">Wert</span><span class="sxs-lookup"><span data-stu-id="9fae7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fae7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fae7-125">Authorization</span></span>|<span data-ttu-id="9fae7-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9fae7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fae7-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9fae7-127">Accept</span></span>|<span data-ttu-id="9fae7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9fae7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fae7-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9fae7-129">Request body</span></span>
<span data-ttu-id="9fae7-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9fae7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fae7-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="9fae7-131">Response</span></span>
<span data-ttu-id="9fae7-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [AndroidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9fae7-132">If successful, this method returns a `200 OK` response code and [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fae7-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9fae7-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="9fae7-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9fae7-134">Request</span></span>
<span data-ttu-id="9fae7-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9fae7-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="9fae7-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="9fae7-136">Response</span></span>
<span data-ttu-id="9fae7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9fae7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





