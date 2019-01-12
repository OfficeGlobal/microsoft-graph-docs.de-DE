---
title: Liste androidWorkProfileGeneralDeviceConfigurations
description: Listeneigenschaften und Beziehungen der AndroidWorkProfileGeneralDeviceConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bba0ef30142afa2e033606f613d7748046a076a0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929739"
---
# <a name="list-androidworkprofilegeneraldeviceconfigurations"></a><span data-ttu-id="4518a-103">Liste androidWorkProfileGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="4518a-103">List androidWorkProfileGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="4518a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4518a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4518a-105">Listeneigenschaften und Beziehungen der [AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="4518a-105">List properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4518a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4518a-106">Prerequisites</span></span>
<span data-ttu-id="4518a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4518a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4518a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4518a-109">Permission type</span></span>|<span data-ttu-id="4518a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4518a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4518a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4518a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4518a-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4518a-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4518a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4518a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4518a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4518a-114">Not supported.</span></span>|
|<span data-ttu-id="4518a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4518a-115">Application</span></span>|<span data-ttu-id="4518a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4518a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4518a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4518a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4518a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4518a-118">Request headers</span></span>
|<span data-ttu-id="4518a-119">Header</span><span class="sxs-lookup"><span data-stu-id="4518a-119">Header</span></span>|<span data-ttu-id="4518a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="4518a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4518a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4518a-121">Authorization</span></span>|<span data-ttu-id="4518a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4518a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4518a-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4518a-123">Accept</span></span>|<span data-ttu-id="4518a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4518a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4518a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4518a-125">Request body</span></span>
<span data-ttu-id="4518a-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4518a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4518a-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="4518a-127">Response</span></span>
<span data-ttu-id="4518a-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4518a-128">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4518a-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4518a-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="4518a-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4518a-130">Request</span></span>
<span data-ttu-id="4518a-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4518a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="4518a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="4518a-132">Response</span></span>
<span data-ttu-id="4518a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4518a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



