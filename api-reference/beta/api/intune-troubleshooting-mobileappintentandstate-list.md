---
title: MobileAppIntentAndStates aufListen
description: AufListen von Eigenschaften und Beziehungen der mobileAppIntentAndState-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a7c0699af0b7d4ea019ab6d18b2c61c44451cf74
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962694"
---
# <a name="list-mobileappintentandstates"></a><span data-ttu-id="b01a4-103">MobileAppIntentAndStates aufListen</span><span class="sxs-lookup"><span data-stu-id="b01a4-103">List mobileAppIntentAndStates</span></span>

> <span data-ttu-id="b01a4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b01a4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b01a4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b01a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b01a4-106">AufListen von Eigenschaften und Beziehungen der [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="b01a4-106">List properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b01a4-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b01a4-107">Prerequisites</span></span>
<span data-ttu-id="b01a4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b01a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b01a4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b01a4-110">Permission type</span></span>|<span data-ttu-id="b01a4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b01a4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b01a4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b01a4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b01a4-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b01a4-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b01a4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b01a4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b01a4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b01a4-115">Not supported.</span></span>|
|<span data-ttu-id="b01a4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b01a4-116">Application</span></span>|<span data-ttu-id="b01a4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b01a4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b01a4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b01a4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a><span data-ttu-id="b01a4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b01a4-119">Request headers</span></span>
|<span data-ttu-id="b01a4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b01a4-120">Header</span></span>|<span data-ttu-id="b01a4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b01a4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b01a4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b01a4-122">Authorization</span></span>|<span data-ttu-id="b01a4-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b01a4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b01a4-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b01a4-124">Accept</span></span>|<span data-ttu-id="b01a4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b01a4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b01a4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b01a4-126">Request body</span></span>
<span data-ttu-id="b01a4-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b01a4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b01a4-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="b01a4-128">Response</span></span>
<span data-ttu-id="b01a4-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b01a4-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b01a4-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b01a4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b01a4-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b01a4-131">Request</span></span>
<span data-ttu-id="b01a4-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b01a4-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates
```

### <a name="response"></a><span data-ttu-id="b01a4-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="b01a4-133">Response</span></span>
<span data-ttu-id="b01a4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b01a4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




