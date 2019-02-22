---
title: Auflisten von „managedAppStatus“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs managedAppStatus auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00f5cdc90e439a4f4a73d2a979b5f08446d0a161
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143792"
---
# <a name="list-managedappstatuses"></a><span data-ttu-id="8d271-103">Auflisten von „managedAppStatus“</span><span class="sxs-lookup"><span data-stu-id="8d271-103">List managedAppStatuses</span></span>

> <span data-ttu-id="8d271-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8d271-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d271-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8d271-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d271-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedAppStatus](../resources/intune-mam-managedappstatus.md) auf.</span><span class="sxs-lookup"><span data-stu-id="8d271-106">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d271-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8d271-107">Prerequisites</span></span>
<span data-ttu-id="8d271-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8d271-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8d271-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8d271-110">Permission type</span></span>|<span data-ttu-id="8d271-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8d271-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d271-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8d271-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d271-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d271-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8d271-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8d271-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d271-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d271-115">Not supported.</span></span>|
|<span data-ttu-id="8d271-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8d271-116">Application</span></span>|<span data-ttu-id="8d271-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d271-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d271-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d271-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="8d271-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8d271-119">Request headers</span></span>
|<span data-ttu-id="8d271-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8d271-120">Header</span></span>|<span data-ttu-id="8d271-121">Wert</span><span class="sxs-lookup"><span data-stu-id="8d271-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d271-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d271-122">Authorization</span></span>|<span data-ttu-id="8d271-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8d271-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d271-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8d271-124">Accept</span></span>|<span data-ttu-id="8d271-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8d271-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d271-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8d271-126">Request body</span></span>
<span data-ttu-id="8d271-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8d271-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d271-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d271-128">Response</span></span>
<span data-ttu-id="8d271-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAppStatus](../resources/intune-mam-managedappstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8d271-129">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d271-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8d271-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d271-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d271-131">Request</span></span>
<span data-ttu-id="8d271-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8d271-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="8d271-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d271-133">Response</span></span>
<span data-ttu-id="8d271-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d271-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 227

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppStatus",
      "displayName": "Display Name value",
      "id": "ad1f7541-7541-ad1f-4175-1fad41751fad",
      "version": "Version value"
    }
  ]
}
```




