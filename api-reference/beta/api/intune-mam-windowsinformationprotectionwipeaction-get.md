---
title: WindowsInformationProtectionWipeAction abrufen
description: Lesen von Eigenschaften und Beziehungen des windowsInformationProtectionWipeAction-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ad145cccf75ffad4abf8a939306e178440118b49
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977569"
---
# <a name="get-windowsinformationprotectionwipeaction"></a><span data-ttu-id="24c80-103">WindowsInformationProtectionWipeAction abrufen</span><span class="sxs-lookup"><span data-stu-id="24c80-103">Get windowsInformationProtectionWipeAction</span></span>

> <span data-ttu-id="24c80-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="24c80-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24c80-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="24c80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24c80-106">Lesen von Eigenschaften und Beziehungen des [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="24c80-106">Read properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24c80-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="24c80-107">Prerequisites</span></span>
<span data-ttu-id="24c80-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24c80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24c80-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="24c80-110">Permission type</span></span>|<span data-ttu-id="24c80-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="24c80-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24c80-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="24c80-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24c80-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="24c80-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="24c80-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="24c80-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24c80-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="24c80-115">Not supported.</span></span>|
|<span data-ttu-id="24c80-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="24c80-116">Application</span></span>|<span data-ttu-id="24c80-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="24c80-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24c80-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="24c80-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24c80-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="24c80-119">Optional query parameters</span></span>
<span data-ttu-id="24c80-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="24c80-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24c80-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="24c80-121">Request headers</span></span>
|<span data-ttu-id="24c80-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="24c80-122">Header</span></span>|<span data-ttu-id="24c80-123">Wert</span><span class="sxs-lookup"><span data-stu-id="24c80-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24c80-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="24c80-124">Authorization</span></span>|<span data-ttu-id="24c80-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="24c80-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24c80-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="24c80-126">Accept</span></span>|<span data-ttu-id="24c80-127">application/json</span><span class="sxs-lookup"><span data-stu-id="24c80-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24c80-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="24c80-128">Request body</span></span>
<span data-ttu-id="24c80-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="24c80-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24c80-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="24c80-130">Response</span></span>
<span data-ttu-id="24c80-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="24c80-131">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24c80-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="24c80-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="24c80-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="24c80-133">Request</span></span>
<span data-ttu-id="24c80-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="24c80-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

### <a name="response"></a><span data-ttu-id="24c80-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="24c80-135">Response</span></span>
<span data-ttu-id="24c80-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="24c80-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 496

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
    "id": "2620a996-a996-2620-96a9-202696a92026",
    "status": "pending",
    "targetedUserId": "Targeted User Id value",
    "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
    "targetedDeviceName": "Targeted Device Name value",
    "targetedDeviceMacAddress": "Targeted Device Mac Address value",
    "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
  }
}
```




