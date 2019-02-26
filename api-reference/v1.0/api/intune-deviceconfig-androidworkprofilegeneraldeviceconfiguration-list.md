---
title: AndroidWorkProfileGeneralDeviceConfigurations aufListen
description: AufListen von Eigenschaften und Beziehungen der androidWorkProfileGeneralDeviceConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4f821208383f6dece05433f8541e5be2fcfc3acd
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250782"
---
# <a name="list-androidworkprofilegeneraldeviceconfigurations"></a><span data-ttu-id="b68b3-103">AndroidWorkProfileGeneralDeviceConfigurations aufListen</span><span class="sxs-lookup"><span data-stu-id="b68b3-103">List androidWorkProfileGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="b68b3-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b68b3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b68b3-105">AufListen von Eigenschaften und Beziehungen der [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="b68b3-105">List properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b68b3-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b68b3-106">Prerequisites</span></span>
<span data-ttu-id="b68b3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b68b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b68b3-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b68b3-109">Permission type</span></span>|<span data-ttu-id="b68b3-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b68b3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b68b3-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b68b3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b68b3-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b68b3-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b68b3-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b68b3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b68b3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b68b3-114">Not supported.</span></span>|
|<span data-ttu-id="b68b3-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b68b3-115">Application</span></span>|<span data-ttu-id="b68b3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b68b3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b68b3-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b68b3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b68b3-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b68b3-118">Request headers</span></span>
|<span data-ttu-id="b68b3-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b68b3-119">Header</span></span>|<span data-ttu-id="b68b3-120">Wert</span><span class="sxs-lookup"><span data-stu-id="b68b3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b68b3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b68b3-121">Authorization</span></span>|<span data-ttu-id="b68b3-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b68b3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b68b3-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b68b3-123">Accept</span></span>|<span data-ttu-id="b68b3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b68b3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b68b3-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b68b3-125">Request body</span></span>
<span data-ttu-id="b68b3-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b68b3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b68b3-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="b68b3-127">Response</span></span>
<span data-ttu-id="b68b3-128">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b68b3-128">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b68b3-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b68b3-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="b68b3-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b68b3-130">Request</span></span>
<span data-ttu-id="b68b3-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b68b3-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="b68b3-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b68b3-132">Response</span></span>
<span data-ttu-id="b68b3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b68b3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



