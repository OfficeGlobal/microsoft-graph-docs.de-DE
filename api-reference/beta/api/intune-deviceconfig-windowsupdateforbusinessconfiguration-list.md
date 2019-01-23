---
title: Auflisten von „windowsUpdateForBusinessConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windowsUpdateForBusinessConfiguration auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d3da41b3b29fb7cc65b643435299b0302d2aa6e2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396917"
---
# <a name="list-windowsupdateforbusinessconfigurations"></a><span data-ttu-id="dcfbb-103">Auflisten von „windowsUpdateForBusinessConfiguration“</span><span class="sxs-lookup"><span data-stu-id="dcfbb-103">List windowsUpdateForBusinessConfigurations</span></span>

> <span data-ttu-id="dcfbb-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="dcfbb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dcfbb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dcfbb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dcfbb-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dcfbb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcfbb-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="dcfbb-107">List properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dcfbb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dcfbb-108">Prerequisites</span></span>
<span data-ttu-id="dcfbb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dcfbb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dcfbb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dcfbb-111">Permission type</span></span>|<span data-ttu-id="dcfbb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dcfbb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dcfbb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dcfbb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dcfbb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcfbb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dcfbb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dcfbb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcfbb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dcfbb-116">Not supported.</span></span>|
|<span data-ttu-id="dcfbb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dcfbb-117">Application</span></span>|<span data-ttu-id="dcfbb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dcfbb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcfbb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dcfbb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="dcfbb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dcfbb-120">Request headers</span></span>
|<span data-ttu-id="dcfbb-121">Header</span><span class="sxs-lookup"><span data-stu-id="dcfbb-121">Header</span></span>|<span data-ttu-id="dcfbb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="dcfbb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dcfbb-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="dcfbb-123">Authorization</span></span>|<span data-ttu-id="dcfbb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dcfbb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dcfbb-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dcfbb-125">Accept</span></span>|<span data-ttu-id="dcfbb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dcfbb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcfbb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dcfbb-127">Request body</span></span>
<span data-ttu-id="dcfbb-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dcfbb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcfbb-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="dcfbb-129">Response</span></span>
<span data-ttu-id="dcfbb-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="dcfbb-130">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcfbb-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dcfbb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcfbb-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dcfbb-132">Request</span></span>
<span data-ttu-id="dcfbb-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dcfbb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="dcfbb-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="dcfbb-134">Response</span></span>
<span data-ttu-id="dcfbb-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dcfbb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2185

{
  "value": [
    {
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
      "userPauseAccess": "enabled"
    }
  ]
}
```




