---
title: Abrufen von „windowsUpdateForBusinessConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs windowsUpdateForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 10af8dbfb47d03ace56d5b6542f8f47651fe19c7
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30570696"
---
# <a name="get-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="dd981-103">Abrufen von „windowsUpdateForBusinessConfiguration“</span><span class="sxs-lookup"><span data-stu-id="dd981-103">Get windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="dd981-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dd981-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd981-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="dd981-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd981-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd981-106">Read properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd981-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dd981-107">Prerequisites</span></span>
<span data-ttu-id="dd981-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dd981-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dd981-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dd981-110">Permission type</span></span>|<span data-ttu-id="dd981-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dd981-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd981-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dd981-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dd981-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd981-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dd981-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dd981-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd981-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd981-115">Not supported.</span></span>|
|<span data-ttu-id="dd981-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dd981-116">Application</span></span>|<span data-ttu-id="dd981-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd981-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd981-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd981-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dd981-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="dd981-119">Optional query parameters</span></span>
<span data-ttu-id="dd981-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dd981-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd981-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dd981-121">Request headers</span></span>
|<span data-ttu-id="dd981-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dd981-122">Header</span></span>|<span data-ttu-id="dd981-123">Wert</span><span class="sxs-lookup"><span data-stu-id="dd981-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd981-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd981-124">Authorization</span></span>|<span data-ttu-id="dd981-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dd981-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd981-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dd981-126">Accept</span></span>|<span data-ttu-id="dd981-127">application/json</span><span class="sxs-lookup"><span data-stu-id="dd981-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd981-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dd981-128">Request body</span></span>
<span data-ttu-id="dd981-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dd981-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd981-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd981-130">Response</span></span>
<span data-ttu-id="dd981-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="dd981-131">If successful, this method returns a `200 OK` response code and [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd981-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dd981-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd981-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd981-133">Request</span></span>
<span data-ttu-id="dd981-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dd981-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="dd981-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd981-135">Response</span></span>
<span data-ttu-id="dd981-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd981-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2186

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
    "id": "4928dd6a-dd6a-4928-6add-28496add2849",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "deliveryOptimizationMode": "httpOnly",
    "prereleaseFeatures": "settingsOnly",
    "automaticUpdateMode": "notifyDownload",
    "microsoftUpdateServiceAllowed": true,
    "driversExcluded": true,
    "installationSchedule": {
      "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
      "scheduledInstallDay": "everyday",
      "scheduledInstallTime": "11:59:31.3170000"
    },
    "qualityUpdatesDeferralPeriodInDays": 2,
    "featureUpdatesDeferralPeriodInDays": 2,
    "qualityUpdatesPaused": true,
    "featureUpdatesPaused": true,
    "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
    "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
    "businessReadyUpdatesOnly": "all",
    "skipChecksBeforeRestart": true,
    "updateWeeks": "firstWeek",
    "qualityUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
    "featureUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
    "featureUpdatesRollbackWindowInDays": 2,
    "qualityUpdatesWillBeRolledBack": true,
    "featureUpdatesWillBeRolledBack": true,
    "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
    "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
    "engagedRestartDeadlineInDays": 12,
    "engagedRestartSnoozeScheduleInDays": 2,
    "engagedRestartTransitionScheduleInDays": 6,
    "autoRestartNotificationDismissal": "automatic",
    "scheduleRestartWarningInHours": 13,
    "scheduleImminentRestartWarningInMinutes": 7,
    "userPauseAccess": "enabled",
    "userWindowsUpdateScanAccess": "enabled",
    "updateNotificationLevel": "defaultNotifications"
  }
}
```




