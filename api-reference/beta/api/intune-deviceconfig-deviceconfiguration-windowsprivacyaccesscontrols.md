---
title: windowsPrivacyAccessControls-Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 38b6cabb42c71beb5095f9fd97827f1ddb396e5c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142385"
---
# <a name="windowsprivacyaccesscontrols-action"></a><span data-ttu-id="66bdc-103">windowsPrivacyAccessControls-Aktion</span><span class="sxs-lookup"><span data-stu-id="66bdc-103">windowsPrivacyAccessControls action</span></span>

> <span data-ttu-id="66bdc-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="66bdc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66bdc-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="66bdc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66bdc-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="66bdc-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66bdc-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="66bdc-107">Prerequisites</span></span>
<span data-ttu-id="66bdc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="66bdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="66bdc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="66bdc-110">Permission type</span></span>|<span data-ttu-id="66bdc-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="66bdc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66bdc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="66bdc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66bdc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66bdc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="66bdc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="66bdc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66bdc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66bdc-115">Not supported.</span></span>|
|<span data-ttu-id="66bdc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="66bdc-116">Application</span></span>|<span data-ttu-id="66bdc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66bdc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66bdc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="66bdc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/windowsPrivacyAccessControls
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/windowsPrivacyAccessControls
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/windowsPrivacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="66bdc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="66bdc-119">Request headers</span></span>
|<span data-ttu-id="66bdc-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="66bdc-120">Header</span></span>|<span data-ttu-id="66bdc-121">Wert</span><span class="sxs-lookup"><span data-stu-id="66bdc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66bdc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="66bdc-122">Authorization</span></span>|<span data-ttu-id="66bdc-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="66bdc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66bdc-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="66bdc-124">Accept</span></span>|<span data-ttu-id="66bdc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="66bdc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66bdc-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="66bdc-126">Request body</span></span>
<span data-ttu-id="66bdc-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="66bdc-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="66bdc-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="66bdc-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="66bdc-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="66bdc-129">Property</span></span>|<span data-ttu-id="66bdc-130">Typ</span><span class="sxs-lookup"><span data-stu-id="66bdc-130">Type</span></span>|<span data-ttu-id="66bdc-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66bdc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66bdc-132">windowsPrivacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="66bdc-132">windowsPrivacyAccessControls</span></span>|<span data-ttu-id="66bdc-133">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="66bdc-133">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="66bdc-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="66bdc-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="66bdc-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="66bdc-135">Response</span></span>
<span data-ttu-id="66bdc-136">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="66bdc-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="66bdc-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="66bdc-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="66bdc-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="66bdc-138">Request</span></span>
<span data-ttu-id="66bdc-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="66bdc-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/windowsPrivacyAccessControls

Content-type: application/json
Content-length: 379

{
  "windowsPrivacyAccessControls": [
    {
      "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
      "id": "03b15556-5556-03b1-5655-b1035655b103",
      "accessLevel": "forceAllow",
      "dataCategory": "accountInfo",
      "appPackageFamilyName": "App Package Family Name value",
      "appDisplayName": "App Display Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="66bdc-140">Reaktion</span><span class="sxs-lookup"><span data-stu-id="66bdc-140">Response</span></span>
<span data-ttu-id="66bdc-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="66bdc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




