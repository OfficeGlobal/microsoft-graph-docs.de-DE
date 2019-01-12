---
title: Auflisten von „managedDeviceMobileAppConfigurationUserStatus“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs managedDeviceMobileAppConfigurationUserStatus auf.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fc0d0462ea4355c5e3f5b914419da9a17d43e45e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929613"
---
# <a name="list-manageddevicemobileappconfigurationuserstatuses"></a><span data-ttu-id="53eca-103">Auflisten von „managedDeviceMobileAppConfigurationUserStatus“</span><span class="sxs-lookup"><span data-stu-id="53eca-103">List managedDeviceMobileAppConfigurationUserStatuses</span></span>

> <span data-ttu-id="53eca-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="53eca-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53eca-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) auf.</span><span class="sxs-lookup"><span data-stu-id="53eca-105">List properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="53eca-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="53eca-106">Prerequisites</span></span>
<span data-ttu-id="53eca-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53eca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53eca-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53eca-109">Permission type</span></span>|<span data-ttu-id="53eca-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53eca-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53eca-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53eca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="53eca-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="53eca-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="53eca-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53eca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53eca-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53eca-114">Not supported.</span></span>|
|<span data-ttu-id="53eca-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53eca-115">Application</span></span>|<span data-ttu-id="53eca-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53eca-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53eca-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53eca-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="53eca-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53eca-118">Request headers</span></span>
|<span data-ttu-id="53eca-119">Header</span><span class="sxs-lookup"><span data-stu-id="53eca-119">Header</span></span>|<span data-ttu-id="53eca-120">Wert</span><span class="sxs-lookup"><span data-stu-id="53eca-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53eca-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="53eca-121">Authorization</span></span>|<span data-ttu-id="53eca-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="53eca-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53eca-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="53eca-123">Accept</span></span>|<span data-ttu-id="53eca-124">application/json</span><span class="sxs-lookup"><span data-stu-id="53eca-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53eca-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53eca-125">Request body</span></span>
<span data-ttu-id="53eca-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="53eca-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53eca-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="53eca-127">Response</span></span>
<span data-ttu-id="53eca-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="53eca-128">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53eca-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53eca-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="53eca-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53eca-130">Request</span></span>
<span data-ttu-id="53eca-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="53eca-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="53eca-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="53eca-132">Response</span></span>
<span data-ttu-id="53eca-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53eca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 416

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
      "id": "44960944-0944-4496-4409-964444099644",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



