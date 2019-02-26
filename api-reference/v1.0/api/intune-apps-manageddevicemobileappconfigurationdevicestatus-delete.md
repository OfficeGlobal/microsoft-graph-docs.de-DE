---
title: ManagedDeviceMobileAppConfigurationDeviceStatus löschen
description: Löscht eine managedDeviceMobileAppConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3eedec45296884829a476cd5a8acc051d6af62d6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264148"
---
# <a name="delete-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="0b632-103">ManagedDeviceMobileAppConfigurationDeviceStatus löschen</span><span class="sxs-lookup"><span data-stu-id="0b632-103">Delete managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="0b632-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0b632-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b632-105">Löscht eine [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="0b632-105">Deletes a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b632-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0b632-106">Prerequisites</span></span>
<span data-ttu-id="0b632-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0b632-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0b632-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0b632-109">Permission type</span></span>|<span data-ttu-id="0b632-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0b632-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b632-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0b632-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0b632-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b632-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0b632-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0b632-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b632-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b632-114">Not supported.</span></span>|
|<span data-ttu-id="0b632-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0b632-115">Application</span></span>|<span data-ttu-id="0b632-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b632-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b632-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b632-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="0b632-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0b632-118">Request headers</span></span>
|<span data-ttu-id="0b632-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0b632-119">Header</span></span>|<span data-ttu-id="0b632-120">Wert</span><span class="sxs-lookup"><span data-stu-id="0b632-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b632-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b632-121">Authorization</span></span>|<span data-ttu-id="0b632-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0b632-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b632-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0b632-123">Accept</span></span>|<span data-ttu-id="0b632-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0b632-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b632-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0b632-125">Request body</span></span>
<span data-ttu-id="0b632-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0b632-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b632-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b632-127">Response</span></span>
<span data-ttu-id="0b632-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0b632-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0b632-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0b632-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b632-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b632-130">Request</span></span>
<span data-ttu-id="0b632-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0b632-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="0b632-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b632-132">Response</span></span>
<span data-ttu-id="0b632-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0b632-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



