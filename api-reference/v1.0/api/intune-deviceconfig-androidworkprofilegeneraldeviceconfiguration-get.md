---
title: Abrufen von androidWorkProfileGeneralDeviceConfiguration
description: Lesen Sie Eigenschaften und Beziehungen des AndroidWorkProfileGeneralDeviceConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d1ce36a8684a269be92523c590f07b2065673def
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883839"
---
# <a name="get-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="3241c-103">Abrufen von androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3241c-103">Get androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="3241c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3241c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3241c-105">Lesen Sie Eigenschaften und Beziehungen des [AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3241c-105">Read properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3241c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3241c-106">Prerequisites</span></span>
<span data-ttu-id="3241c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3241c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3241c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3241c-109">Permission type</span></span>|<span data-ttu-id="3241c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3241c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3241c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3241c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3241c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3241c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3241c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3241c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3241c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3241c-114">Not supported.</span></span>|
|<span data-ttu-id="3241c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3241c-115">Application</span></span>|<span data-ttu-id="3241c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3241c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3241c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3241c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3241c-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3241c-118">Optional query parameters</span></span>
<span data-ttu-id="3241c-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3241c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3241c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3241c-120">Request headers</span></span>
|<span data-ttu-id="3241c-121">Header</span><span class="sxs-lookup"><span data-stu-id="3241c-121">Header</span></span>|<span data-ttu-id="3241c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3241c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3241c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3241c-123">Authorization</span></span>|<span data-ttu-id="3241c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3241c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3241c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3241c-125">Accept</span></span>|<span data-ttu-id="3241c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3241c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3241c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3241c-127">Request body</span></span>
<span data-ttu-id="3241c-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3241c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3241c-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3241c-129">Response</span></span>
<span data-ttu-id="3241c-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3241c-130">If successful, this method returns a `200 OK` response code and [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3241c-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3241c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3241c-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3241c-132">Request</span></span>
<span data-ttu-id="3241c-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3241c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="3241c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3241c-134">Response</span></span>
<span data-ttu-id="3241c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3241c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



