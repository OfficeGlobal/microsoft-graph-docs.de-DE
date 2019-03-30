---
title: iosUpdateConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des iosUpdateConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3cf8cfce47708727270ca536d20a62813473da6c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989547"
---
# <a name="get-iosupdateconfiguration"></a><span data-ttu-id="6d756-103">iosUpdateConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="6d756-103">Get iosUpdateConfiguration</span></span>

> <span data-ttu-id="6d756-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6d756-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d756-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6d756-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d756-106">Lesen von Eigenschaften und Beziehungen des [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6d756-106">Read properties and relationships of the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d756-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6d756-107">Prerequisites</span></span>
<span data-ttu-id="6d756-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d756-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d756-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6d756-110">Permission type</span></span>|<span data-ttu-id="6d756-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6d756-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d756-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6d756-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6d756-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d756-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6d756-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6d756-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d756-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6d756-115">Not supported.</span></span>|
|<span data-ttu-id="6d756-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6d756-116">Application</span></span>|<span data-ttu-id="6d756-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6d756-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d756-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d756-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d756-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6d756-119">Optional query parameters</span></span>
<span data-ttu-id="6d756-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6d756-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d756-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6d756-121">Request headers</span></span>
|<span data-ttu-id="6d756-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6d756-122">Header</span></span>|<span data-ttu-id="6d756-123">Wert</span><span class="sxs-lookup"><span data-stu-id="6d756-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d756-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d756-124">Authorization</span></span>|<span data-ttu-id="6d756-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6d756-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d756-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6d756-126">Accept</span></span>|<span data-ttu-id="6d756-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6d756-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d756-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6d756-128">Request body</span></span>
<span data-ttu-id="6d756-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6d756-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d756-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d756-130">Response</span></span>
<span data-ttu-id="6d756-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6d756-131">If successful, this method returns a `200 OK` response code and [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d756-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6d756-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d756-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d756-133">Request</span></span>
<span data-ttu-id="6d756-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6d756-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="6d756-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d756-135">Response</span></span>
<span data-ttu-id="6d756-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6d756-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 711

{
  "value": {
    "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
    "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "isEnabled": true,
    "activeHoursStart": "12:00:05.5020000",
    "activeHoursEnd": "11:59:00.8990000",
    "scheduledInstallDays": [
      "monday"
    ],
    "utcTimeOffsetInMinutes": 6,
    "enforcedSoftwareUpdateDelayInDays": 1
  }
}
```




