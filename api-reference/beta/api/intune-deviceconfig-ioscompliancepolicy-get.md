---
title: iosCompliancePolicy abrufen
description: Lesen von Eigenschaften und Beziehungen des iosCompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a6f8a85f3a943547ac097539bfce6d9fde07834
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155426"
---
# <a name="get-ioscompliancepolicy"></a><span data-ttu-id="79c97-103">iosCompliancePolicy abrufen</span><span class="sxs-lookup"><span data-stu-id="79c97-103">Get iosCompliancePolicy</span></span>

> <span data-ttu-id="79c97-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="79c97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79c97-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="79c97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79c97-106">Lesen von Eigenschaften und Beziehungen des [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="79c97-106">Read properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79c97-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="79c97-107">Prerequisites</span></span>
<span data-ttu-id="79c97-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="79c97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="79c97-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="79c97-110">Permission type</span></span>|<span data-ttu-id="79c97-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="79c97-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79c97-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="79c97-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79c97-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="79c97-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="79c97-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="79c97-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79c97-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79c97-115">Not supported.</span></span>|
|<span data-ttu-id="79c97-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="79c97-116">Application</span></span>|<span data-ttu-id="79c97-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79c97-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79c97-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="79c97-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79c97-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="79c97-119">Optional query parameters</span></span>
<span data-ttu-id="79c97-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="79c97-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79c97-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="79c97-121">Request headers</span></span>
|<span data-ttu-id="79c97-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="79c97-122">Header</span></span>|<span data-ttu-id="79c97-123">Wert</span><span class="sxs-lookup"><span data-stu-id="79c97-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79c97-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="79c97-124">Authorization</span></span>|<span data-ttu-id="79c97-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="79c97-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79c97-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="79c97-126">Accept</span></span>|<span data-ttu-id="79c97-127">application/json</span><span class="sxs-lookup"><span data-stu-id="79c97-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79c97-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="79c97-128">Request body</span></span>
<span data-ttu-id="79c97-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="79c97-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79c97-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="79c97-130">Response</span></span>
<span data-ttu-id="79c97-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79c97-131">If successful, this method returns a `200 OK` response code and [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79c97-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="79c97-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="79c97-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="79c97-133">Request</span></span>
<span data-ttu-id="79c97-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="79c97-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="79c97-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="79c97-135">Response</span></span>
<span data-ttu-id="79c97-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79c97-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1504

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "4f501351-1351-4f50-5113-504f5113504f",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passcodeBlockSimple": true,
    "passcodeExpirationDays": 6,
    "passcodeMinimumLength": 5,
    "passcodeMinutesOfInactivityBeforeLock": 5,
    "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
    "passcodePreviousPasscodeBlockCount": 2,
    "passcodeMinimumCharacterSetCount": 0,
    "passcodeRequiredType": "alphanumeric",
    "passcodeRequired": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "osMinimumBuildVersion": "Os Minimum Build Version value",
    "osMaximumBuildVersion": "Os Maximum Build Version value",
    "securityBlockJailbrokenDevices": true,
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "managedEmailProfileRequired": true,
    "restrictedApps": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ]
  }
}
```




