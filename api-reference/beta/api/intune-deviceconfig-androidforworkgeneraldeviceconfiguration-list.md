---
title: Liste androidForWorkGeneralDeviceConfigurations
description: Listeneigenschaften und Beziehungen der AndroidForWorkGeneralDeviceConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 44880be8c782697e0eb84743fb3fb249235ac2d3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933708"
---
# <a name="list-androidforworkgeneraldeviceconfigurations"></a><span data-ttu-id="8fb94-103">Liste androidForWorkGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="8fb94-103">List androidForWorkGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="8fb94-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8fb94-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8fb94-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8fb94-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8fb94-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8fb94-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8fb94-107">Listeneigenschaften und Beziehungen der [AndroidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="8fb94-107">List properties and relationships of the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8fb94-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8fb94-108">Prerequisites</span></span>
<span data-ttu-id="8fb94-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fb94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fb94-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8fb94-111">Permission type</span></span>|<span data-ttu-id="8fb94-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8fb94-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fb94-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8fb94-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8fb94-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8fb94-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8fb94-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8fb94-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fb94-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8fb94-116">Not supported.</span></span>|
|<span data-ttu-id="8fb94-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8fb94-117">Application</span></span>|<span data-ttu-id="8fb94-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8fb94-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fb94-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8fb94-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8fb94-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8fb94-120">Request headers</span></span>
|<span data-ttu-id="8fb94-121">Header</span><span class="sxs-lookup"><span data-stu-id="8fb94-121">Header</span></span>|<span data-ttu-id="8fb94-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8fb94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fb94-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fb94-123">Authorization</span></span>|<span data-ttu-id="8fb94-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8fb94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fb94-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8fb94-125">Accept</span></span>|<span data-ttu-id="8fb94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8fb94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fb94-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8fb94-127">Request body</span></span>
<span data-ttu-id="8fb94-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8fb94-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fb94-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8fb94-129">Response</span></span>
<span data-ttu-id="8fb94-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AndroidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8fb94-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fb94-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8fb94-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8fb94-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8fb94-132">Request</span></span>
<span data-ttu-id="8fb94-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8fb94-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="8fb94-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8fb94-134">Response</span></span>
<span data-ttu-id="8fb94-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8fb94-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2431

{
  "value": [
    {
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
  ]
}
```





