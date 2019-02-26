---
title: Abrufen von „windows10TeamGeneralConfiguration“
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs windows10TeamGeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4922352cf9824683b18fe068bfea29b8cb86310b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157435"
---
# <a name="get-windows10teamgeneralconfiguration"></a><span data-ttu-id="aab32-103">Abrufen von „windows10TeamGeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="aab32-103">Get windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="aab32-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aab32-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aab32-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="aab32-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aab32-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aab32-106">Read properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aab32-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="aab32-107">Prerequisites</span></span>
<span data-ttu-id="aab32-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="aab32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="aab32-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aab32-110">Permission type</span></span>|<span data-ttu-id="aab32-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aab32-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aab32-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aab32-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aab32-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="aab32-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="aab32-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aab32-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aab32-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aab32-115">Not supported.</span></span>|
|<span data-ttu-id="aab32-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aab32-116">Application</span></span>|<span data-ttu-id="aab32-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aab32-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aab32-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aab32-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aab32-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="aab32-119">Optional query parameters</span></span>
<span data-ttu-id="aab32-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aab32-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aab32-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aab32-121">Request headers</span></span>
|<span data-ttu-id="aab32-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="aab32-122">Header</span></span>|<span data-ttu-id="aab32-123">Wert</span><span class="sxs-lookup"><span data-stu-id="aab32-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aab32-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="aab32-124">Authorization</span></span>|<span data-ttu-id="aab32-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="aab32-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aab32-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="aab32-126">Accept</span></span>|<span data-ttu-id="aab32-127">application/json</span><span class="sxs-lookup"><span data-stu-id="aab32-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aab32-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aab32-128">Request body</span></span>
<span data-ttu-id="aab32-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="aab32-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aab32-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="aab32-130">Response</span></span>
<span data-ttu-id="aab32-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="aab32-131">If successful, this method returns a `200 OK` response code and [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aab32-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aab32-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="aab32-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aab32-133">Request</span></span>
<span data-ttu-id="aab32-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aab32-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="aab32-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="aab32-135">Response</span></span>
<span data-ttu-id="aab32-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aab32-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1495

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
    "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "azureOperationalInsightsBlockTelemetry": true,
    "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
    "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
    "connectAppBlockAutoLaunch": true,
    "maintenanceWindowBlocked": true,
    "maintenanceWindowDurationInHours": 0,
    "maintenanceWindowStartTime": "11:59:09.3130000",
    "miracastChannel": "one",
    "miracastBlocked": true,
    "miracastRequirePin": true,
    "settingsBlockMyMeetingsAndFiles": true,
    "settingsBlockSessionResume": true,
    "settingsBlockSigninSuggestions": true,
    "settingsDefaultVolume": 5,
    "settingsScreenTimeoutInMinutes": 14,
    "settingsSessionTimeoutInMinutes": 15,
    "settingsSleepTimeoutInMinutes": 13,
    "welcomeScreenBlockAutomaticWakeUp": true,
    "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
    "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
  }
}
```




