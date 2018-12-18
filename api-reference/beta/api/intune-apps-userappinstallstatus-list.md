---
title: Liste userAppInstallStatuses
description: Listeneigenschaften und Beziehungen der UserAppInstallStatus-Objekte.
author: tfitzmac
ms.openlocfilehash: 0aeef4d97e63c42e11fefdb84a4dfb6138fdc6a3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325424"
---
# <a name="list-userappinstallstatuses"></a><span data-ttu-id="4cae8-103">Liste userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="4cae8-103">List userAppInstallStatuses</span></span>

> <span data-ttu-id="4cae8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4cae8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4cae8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4cae8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4cae8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4cae8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4cae8-107">Listeneigenschaften und Beziehungen der [UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="4cae8-107">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4cae8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4cae8-108">Prerequisites</span></span>
<span data-ttu-id="4cae8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cae8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cae8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4cae8-111">Permission type</span></span>|<span data-ttu-id="4cae8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4cae8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cae8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4cae8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4cae8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4cae8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4cae8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4cae8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cae8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4cae8-116">Not supported.</span></span>|
|<span data-ttu-id="4cae8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4cae8-117">Application</span></span>|<span data-ttu-id="4cae8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4cae8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cae8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4cae8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="4cae8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4cae8-120">Request headers</span></span>
|<span data-ttu-id="4cae8-121">Header</span><span class="sxs-lookup"><span data-stu-id="4cae8-121">Header</span></span>|<span data-ttu-id="4cae8-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4cae8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cae8-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4cae8-123">Authorization</span></span>|<span data-ttu-id="4cae8-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4cae8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cae8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4cae8-125">Accept</span></span>|<span data-ttu-id="4cae8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4cae8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cae8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4cae8-127">Request body</span></span>
<span data-ttu-id="4cae8-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4cae8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cae8-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4cae8-129">Response</span></span>
<span data-ttu-id="4cae8-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="4cae8-130">If successful, this method returns a `200 OK` response code and a collection of [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cae8-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4cae8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4cae8-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4cae8-132">Request</span></span>
<span data-ttu-id="4cae8-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4cae8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="4cae8-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4cae8-134">Response</span></span>
<span data-ttu-id="4cae8-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4cae8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





