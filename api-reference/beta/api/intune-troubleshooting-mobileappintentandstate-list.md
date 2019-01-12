---
title: Liste mobileAppIntentAndStates
description: Listeneigenschaften und Beziehungen der MobileAppIntentAndState-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: db08fafb5ab98c77ef30fd315552c76cbe146f86
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978270"
---
# <a name="list-mobileappintentandstates"></a><span data-ttu-id="c0ea6-103">Liste mobileAppIntentAndStates</span><span class="sxs-lookup"><span data-stu-id="c0ea6-103">List mobileAppIntentAndStates</span></span>

> <span data-ttu-id="c0ea6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c0ea6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0ea6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c0ea6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0ea6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c0ea6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0ea6-107">Listeneigenschaften und Beziehungen der [MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="c0ea6-107">List properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c0ea6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c0ea6-108">Prerequisites</span></span>
<span data-ttu-id="c0ea6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0ea6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0ea6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c0ea6-111">Permission type</span></span>|<span data-ttu-id="c0ea6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c0ea6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0ea6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c0ea6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0ea6-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0ea6-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c0ea6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c0ea6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0ea6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0ea6-116">Not supported.</span></span>|
|<span data-ttu-id="c0ea6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c0ea6-117">Application</span></span>|<span data-ttu-id="c0ea6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0ea6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0ea6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0ea6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a><span data-ttu-id="c0ea6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c0ea6-120">Request headers</span></span>
|<span data-ttu-id="c0ea6-121">Header</span><span class="sxs-lookup"><span data-stu-id="c0ea6-121">Header</span></span>|<span data-ttu-id="c0ea6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c0ea6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0ea6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0ea6-123">Authorization</span></span>|<span data-ttu-id="c0ea6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c0ea6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0ea6-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c0ea6-125">Accept</span></span>|<span data-ttu-id="c0ea6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0ea6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0ea6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c0ea6-127">Request body</span></span>
<span data-ttu-id="c0ea6-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c0ea6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0ea6-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0ea6-129">Response</span></span>
<span data-ttu-id="c0ea6-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="c0ea6-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0ea6-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c0ea6-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c0ea6-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0ea6-132">Request</span></span>
<span data-ttu-id="c0ea6-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c0ea6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates
```

### <a name="response"></a><span data-ttu-id="c0ea6-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0ea6-134">Response</span></span>
<span data-ttu-id="c0ea6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0ea6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1001

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
      "id": "45a775d6-75d6-45a7-d675-a745d675a745",
      "managedDeviceIdentifier": "Managed Device Identifier value",
      "userId": "User Id value",
      "mobileAppList": [
        {
          "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
          "applicationId": "Application Id value",
          "displayName": "Display Name value",
          "mobileAppIntent": "notAvailable",
          "displayVersion": "Display Version value",
          "installState": "failed",
          "supportedDeviceTypes": [
            {
              "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
              "type": "windowsRT",
              "minimumOperatingSystemVersion": "Minimum Operating System Version value",
              "maximumOperatingSystemVersion": "Maximum Operating System Version value"
            }
          ]
        }
      ]
    }
  ]
}
```





