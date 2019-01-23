---
title: Auflisten von „managedAppOperation“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs managedAppOperation auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7037047d91a6f1fb67cb5f405dffedaa95ff02b3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412422"
---
# <a name="list-managedappoperations"></a><span data-ttu-id="3474d-103">Auflisten von „managedAppOperation“</span><span class="sxs-lookup"><span data-stu-id="3474d-103">List managedAppOperations</span></span>

> <span data-ttu-id="3474d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="3474d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3474d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3474d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3474d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3474d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3474d-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) auf.</span><span class="sxs-lookup"><span data-stu-id="3474d-107">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3474d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3474d-108">Prerequisites</span></span>
<span data-ttu-id="3474d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3474d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3474d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3474d-111">Permission type</span></span>|<span data-ttu-id="3474d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3474d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3474d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3474d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3474d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3474d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3474d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3474d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3474d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3474d-116">Not supported.</span></span>|
|<span data-ttu-id="3474d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3474d-117">Application</span></span>|<span data-ttu-id="3474d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3474d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3474d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3474d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="3474d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3474d-120">Request headers</span></span>
|<span data-ttu-id="3474d-121">Header</span><span class="sxs-lookup"><span data-stu-id="3474d-121">Header</span></span>|<span data-ttu-id="3474d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3474d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3474d-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3474d-123">Authorization</span></span>|<span data-ttu-id="3474d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3474d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3474d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3474d-125">Accept</span></span>|<span data-ttu-id="3474d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3474d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3474d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3474d-127">Request body</span></span>
<span data-ttu-id="3474d-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3474d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3474d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3474d-129">Response</span></span>
<span data-ttu-id="3474d-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3474d-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3474d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3474d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3474d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3474d-132">Request</span></span>
<span data-ttu-id="3474d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3474d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

### <a name="response"></a><span data-ttu-id="3474d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3474d-134">Response</span></span>
<span data-ttu-id="3474d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3474d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 329

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppOperation",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "state": "State value",
      "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
      "version": "Version value"
    }
  ]
}
```




