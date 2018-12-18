---
title: Auflisten von „windows10TeamGeneralConfiguration“
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs windows10TeamGeneralConfiguration auf.
author: tfitzmac
ms.openlocfilehash: bd438432e5d7cfc97ddd4945e3c2c7ab27d2c9c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329897"
---
# <a name="list-windows10teamgeneralconfigurations"></a><span data-ttu-id="a8bce-103">Auflisten von „windows10TeamGeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="a8bce-103">List windows10TeamGeneralConfigurations</span></span>

> <span data-ttu-id="a8bce-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a8bce-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8bce-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="a8bce-105">List properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a8bce-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a8bce-106">Prerequisites</span></span>
<span data-ttu-id="a8bce-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8bce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8bce-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a8bce-109">Permission type</span></span>|<span data-ttu-id="a8bce-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a8bce-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8bce-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a8bce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a8bce-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8bce-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a8bce-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a8bce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8bce-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8bce-114">Not supported.</span></span>|
|<span data-ttu-id="a8bce-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a8bce-115">Application</span></span>|<span data-ttu-id="a8bce-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8bce-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8bce-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8bce-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a8bce-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a8bce-118">Request headers</span></span>
|<span data-ttu-id="a8bce-119">Header</span><span class="sxs-lookup"><span data-stu-id="a8bce-119">Header</span></span>|<span data-ttu-id="a8bce-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a8bce-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8bce-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a8bce-121">Authorization</span></span>|<span data-ttu-id="a8bce-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a8bce-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8bce-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a8bce-123">Accept</span></span>|<span data-ttu-id="a8bce-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a8bce-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8bce-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a8bce-125">Request body</span></span>
<span data-ttu-id="a8bce-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a8bce-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8bce-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8bce-127">Response</span></span>
<span data-ttu-id="a8bce-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a8bce-128">If successful, this method returns a `200 OK` response code and a collection of [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8bce-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a8bce-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="a8bce-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8bce-130">Request</span></span>
<span data-ttu-id="a8bce-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a8bce-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a8bce-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8bce-132">Response</span></span>
<span data-ttu-id="a8bce-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8bce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1463

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
      "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  ]
}
```



