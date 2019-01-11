---
title: Liste windowsPrivacyDataAccessControlItems
description: Listeneigenschaften und Beziehungen der WindowsPrivacyDataAccessControlItem-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1f6730bd76f0531767f8329ac72671fea1cad364
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862594"
---
# <a name="list-windowsprivacydataaccesscontrolitems"></a><span data-ttu-id="3aa41-103">Liste windowsPrivacyDataAccessControlItems</span><span class="sxs-lookup"><span data-stu-id="3aa41-103">List windowsPrivacyDataAccessControlItems</span></span>

> <span data-ttu-id="3aa41-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3aa41-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3aa41-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3aa41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3aa41-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3aa41-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3aa41-107">Listeneigenschaften und Beziehungen der [WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="3aa41-107">List properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3aa41-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3aa41-108">Prerequisites</span></span>
<span data-ttu-id="3aa41-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3aa41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3aa41-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3aa41-111">Permission type</span></span>|<span data-ttu-id="3aa41-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3aa41-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3aa41-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3aa41-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3aa41-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3aa41-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3aa41-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3aa41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3aa41-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3aa41-116">Not supported.</span></span>|
|<span data-ttu-id="3aa41-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3aa41-117">Application</span></span>|<span data-ttu-id="3aa41-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3aa41-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3aa41-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3aa41-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="3aa41-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3aa41-120">Request headers</span></span>
|<span data-ttu-id="3aa41-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3aa41-121">Header</span></span>|<span data-ttu-id="3aa41-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3aa41-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3aa41-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3aa41-123">Authorization</span></span>|<span data-ttu-id="3aa41-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3aa41-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3aa41-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3aa41-125">Accept</span></span>|<span data-ttu-id="3aa41-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3aa41-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3aa41-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3aa41-127">Request body</span></span>
<span data-ttu-id="3aa41-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3aa41-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3aa41-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3aa41-129">Response</span></span>
<span data-ttu-id="3aa41-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="3aa41-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3aa41-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3aa41-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3aa41-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3aa41-132">Request</span></span>
<span data-ttu-id="3aa41-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3aa41-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

### <a name="response"></a><span data-ttu-id="3aa41-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3aa41-134">Response</span></span>
<span data-ttu-id="3aa41-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3aa41-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "value": [
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





