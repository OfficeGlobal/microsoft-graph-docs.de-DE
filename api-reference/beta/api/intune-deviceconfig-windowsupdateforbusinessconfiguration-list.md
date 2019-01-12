---
title: Auflisten von „windowsUpdateForBusinessConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windowsUpdateForBusinessConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4e5dca771205b2b8d82aff4c85cf96df25003997
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914808"
---
# <a name="list-windowsupdateforbusinessconfigurations"></a><span data-ttu-id="dc420-103">Auflisten von „windowsUpdateForBusinessConfiguration“</span><span class="sxs-lookup"><span data-stu-id="dc420-103">List windowsUpdateForBusinessConfigurations</span></span>

> <span data-ttu-id="dc420-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dc420-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc420-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dc420-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc420-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dc420-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc420-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="dc420-107">List properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dc420-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dc420-108">Prerequisites</span></span>
<span data-ttu-id="dc420-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc420-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc420-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dc420-111">Permission type</span></span>|<span data-ttu-id="dc420-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dc420-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc420-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dc420-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dc420-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc420-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dc420-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dc420-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc420-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dc420-116">Not supported.</span></span>|
|<span data-ttu-id="dc420-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dc420-117">Application</span></span>|<span data-ttu-id="dc420-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dc420-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc420-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dc420-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="dc420-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dc420-120">Request headers</span></span>
|<span data-ttu-id="dc420-121">Header</span><span class="sxs-lookup"><span data-stu-id="dc420-121">Header</span></span>|<span data-ttu-id="dc420-122">Wert</span><span class="sxs-lookup"><span data-stu-id="dc420-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc420-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc420-123">Authorization</span></span>|<span data-ttu-id="dc420-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dc420-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc420-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dc420-125">Accept</span></span>|<span data-ttu-id="dc420-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc420-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc420-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dc420-127">Request body</span></span>
<span data-ttu-id="dc420-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dc420-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc420-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="dc420-129">Response</span></span>
<span data-ttu-id="dc420-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="dc420-130">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc420-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dc420-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="dc420-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dc420-132">Request</span></span>
<span data-ttu-id="dc420-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dc420-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="dc420-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="dc420-134">Response</span></span>
<span data-ttu-id="dc420-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dc420-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2176

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
      "qualityUpdatesPauseStartDateTime": "Quality Updates Pause Start Date Time value",
      "featureUpdatesPauseStartDateTime": "Feature Updates Pause Start Date Time value",
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
      "scheduleImminentRestartWarningInMinutes": 7
    }
  ]
}
```





