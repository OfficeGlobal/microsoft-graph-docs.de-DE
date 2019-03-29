---
title: Abrufen von „managedAppPolicy“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3eafd1efaf4368d81445d103e1d2e16ce012ba1f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957269"
---
# <a name="get-managedapppolicy"></a><span data-ttu-id="e7634-103">Abrufen von „managedAppPolicy“</span><span class="sxs-lookup"><span data-stu-id="e7634-103">Get managedAppPolicy</span></span>

> <span data-ttu-id="e7634-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e7634-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7634-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e7634-105">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7634-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e7634-106">Prerequisites</span></span>
<span data-ttu-id="e7634-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7634-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7634-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e7634-109">Permission type</span></span>|<span data-ttu-id="e7634-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e7634-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7634-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e7634-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e7634-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7634-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e7634-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e7634-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7634-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e7634-114">Not supported.</span></span>|
|<span data-ttu-id="e7634-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e7634-115">Application</span></span>|<span data-ttu-id="e7634-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e7634-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7634-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7634-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e7634-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e7634-118">Optional query parameters</span></span>
<span data-ttu-id="e7634-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e7634-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7634-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e7634-120">Request headers</span></span>
|<span data-ttu-id="e7634-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e7634-121">Header</span></span>|<span data-ttu-id="e7634-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e7634-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7634-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7634-123">Authorization</span></span>|<span data-ttu-id="e7634-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e7634-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7634-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e7634-125">Accept</span></span>|<span data-ttu-id="e7634-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7634-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7634-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e7634-127">Request body</span></span>
<span data-ttu-id="e7634-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e7634-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7634-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7634-129">Response</span></span>
<span data-ttu-id="e7634-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e7634-130">If successful, this method returns a `200 OK` response code and [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7634-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e7634-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7634-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7634-132">Request</span></span>
<span data-ttu-id="e7634-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e7634-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="e7634-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7634-134">Response</span></span>
<span data-ttu-id="e7634-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e7634-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 373

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppPolicy",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
    "version": "Version value"
  }
}
```



