---
title: Abrufen von androidForWorkGeneralDeviceConfiguration
description: Lesen Sie Eigenschaften und Beziehungen des AndroidForWorkGeneralDeviceConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c5abdea1618484ee2ef30b7e9ef5f5c56240d3bd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420437"
---
# <a name="get-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="36534-103">Abrufen von androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="36534-103">Get androidForWorkGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="36534-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="36534-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="36534-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="36534-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36534-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="36534-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36534-107">Lesen Sie Eigenschaften und Beziehungen des [AndroidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="36534-107">Read properties and relationships of the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36534-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="36534-108">Prerequisites</span></span>
<span data-ttu-id="36534-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="36534-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="36534-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="36534-111">Permission type</span></span>|<span data-ttu-id="36534-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="36534-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36534-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="36534-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36534-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="36534-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="36534-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="36534-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36534-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36534-116">Not supported.</span></span>|
|<span data-ttu-id="36534-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="36534-117">Application</span></span>|<span data-ttu-id="36534-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36534-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36534-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="36534-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36534-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="36534-120">Optional query parameters</span></span>
<span data-ttu-id="36534-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="36534-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36534-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="36534-122">Request headers</span></span>
|<span data-ttu-id="36534-123">Header</span><span class="sxs-lookup"><span data-stu-id="36534-123">Header</span></span>|<span data-ttu-id="36534-124">Wert</span><span class="sxs-lookup"><span data-stu-id="36534-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36534-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="36534-125">Authorization</span></span>|<span data-ttu-id="36534-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="36534-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36534-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="36534-127">Accept</span></span>|<span data-ttu-id="36534-128">application/json</span><span class="sxs-lookup"><span data-stu-id="36534-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36534-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="36534-129">Request body</span></span>
<span data-ttu-id="36534-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="36534-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36534-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="36534-131">Response</span></span>
<span data-ttu-id="36534-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [AndroidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="36534-132">If successful, this method returns a `200 OK` response code and [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36534-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="36534-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="36534-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="36534-134">Request</span></span>
<span data-ttu-id="36534-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="36534-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="36534-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="36534-136">Response</span></span>
<span data-ttu-id="36534-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="36534-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




