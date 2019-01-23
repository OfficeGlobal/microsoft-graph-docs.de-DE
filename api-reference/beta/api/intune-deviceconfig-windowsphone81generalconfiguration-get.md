---
title: windowsPhone81GeneralConfiguration abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs windowsPhone81GeneralConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 972aa2f3865d4a8b608343817ec732b013ad412a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397680"
---
# <a name="get-windowsphone81generalconfiguration"></a><span data-ttu-id="50e51-103">windowsPhone81GeneralConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="50e51-103">Get windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="50e51-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="50e51-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="50e51-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="50e51-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50e51-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="50e51-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50e51-107">Liest die Eigenschaften und Beziehungen von Objekten des Typs [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50e51-107">Read properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50e51-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="50e51-108">Prerequisites</span></span>
<span data-ttu-id="50e51-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="50e51-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="50e51-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="50e51-111">Permission type</span></span>|<span data-ttu-id="50e51-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="50e51-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50e51-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="50e51-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50e51-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="50e51-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="50e51-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="50e51-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50e51-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50e51-116">Not supported.</span></span>|
|<span data-ttu-id="50e51-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="50e51-117">Application</span></span>|<span data-ttu-id="50e51-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50e51-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50e51-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="50e51-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="50e51-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="50e51-120">Optional query parameters</span></span>
<span data-ttu-id="50e51-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="50e51-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50e51-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="50e51-122">Request headers</span></span>
|<span data-ttu-id="50e51-123">Header</span><span class="sxs-lookup"><span data-stu-id="50e51-123">Header</span></span>|<span data-ttu-id="50e51-124">Wert</span><span class="sxs-lookup"><span data-stu-id="50e51-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50e51-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="50e51-125">Authorization</span></span>|<span data-ttu-id="50e51-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="50e51-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50e51-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="50e51-127">Accept</span></span>|<span data-ttu-id="50e51-128">application/json</span><span class="sxs-lookup"><span data-stu-id="50e51-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50e51-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="50e51-129">Request body</span></span>
<span data-ttu-id="50e51-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="50e51-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50e51-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="50e51-131">Response</span></span>
<span data-ttu-id="50e51-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="50e51-132">If successful, this method returns a `200 OK` response code and [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50e51-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="50e51-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="50e51-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="50e51-134">Request</span></span>
<span data-ttu-id="50e51-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="50e51-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="50e51-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="50e51-136">Response</span></span>
<span data-ttu-id="50e51-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="50e51-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1840

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
    "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "applyOnlyToWindowsPhone81": true,
    "appsBlockCopyPaste": true,
    "bluetoothBlocked": true,
    "cameraBlocked": true,
    "cellularBlockWifiTethering": true,
    "compliantAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "compliantAppListType": "appsInListCompliant",
    "diagnosticDataBlockSubmission": true,
    "emailBlockAddingAccounts": true,
    "locationServicesBlocked": true,
    "microsoftAccountBlocked": true,
    "nfcBlocked": true,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordMinimumCharacterSetCount": 0,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "passwordRequiredType": "alphanumeric",
    "passwordRequired": true,
    "screenCaptureBlocked": true,
    "storageBlockRemovableStorage": true,
    "storageRequireEncryption": true,
    "webBrowserBlocked": true,
    "wifiBlocked": true,
    "wifiBlockAutomaticConnectHotspots": true,
    "wifiBlockHotspotReporting": true,
    "windowsStoreBlocked": true
  }
}
```




