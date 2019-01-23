---
title: Liste userAppInstallStatuses
description: Listeneigenschaften und Beziehungen der UserAppInstallStatus-Objekte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dc9a58c913a62028056484f3b686984d2a9a34f1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405548"
---
# <a name="list-userappinstallstatuses"></a><span data-ttu-id="a80a7-103">Liste userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="a80a7-103">List userAppInstallStatuses</span></span>

> <span data-ttu-id="a80a7-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a80a7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a80a7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a80a7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a80a7-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a80a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a80a7-107">Listeneigenschaften und Beziehungen der [UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="a80a7-107">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a80a7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a80a7-108">Prerequisites</span></span>
<span data-ttu-id="a80a7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a80a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a80a7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a80a7-111">Permission type</span></span>|<span data-ttu-id="a80a7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a80a7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a80a7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a80a7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a80a7-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a80a7-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a80a7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a80a7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a80a7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a80a7-116">Not supported.</span></span>|
|<span data-ttu-id="a80a7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a80a7-117">Application</span></span>|<span data-ttu-id="a80a7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a80a7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a80a7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a80a7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="a80a7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a80a7-120">Request headers</span></span>
|<span data-ttu-id="a80a7-121">Header</span><span class="sxs-lookup"><span data-stu-id="a80a7-121">Header</span></span>|<span data-ttu-id="a80a7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a80a7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a80a7-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a80a7-123">Authorization</span></span>|<span data-ttu-id="a80a7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a80a7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a80a7-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a80a7-125">Accept</span></span>|<span data-ttu-id="a80a7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a80a7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a80a7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a80a7-127">Request body</span></span>
<span data-ttu-id="a80a7-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a80a7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a80a7-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a80a7-129">Response</span></span>
<span data-ttu-id="a80a7-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="a80a7-130">If successful, this method returns a `200 OK` response code and a collection of [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a80a7-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a80a7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a80a7-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a80a7-132">Request</span></span>
<span data-ttu-id="a80a7-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a80a7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="a80a7-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a80a7-134">Response</span></span>
<span data-ttu-id="a80a7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a80a7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 349

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userAppInstallStatus",
      "id": "14959a2a-9a2a-1495-2a9a-95142a9a9514",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "installedDeviceCount": 4,
      "failedDeviceCount": 1,
      "notInstalledDeviceCount": 7
    }
  ]
}
```




