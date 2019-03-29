---
title: deviceEnrollmentConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceEnrollmentConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c883705935500293e504d097f939029c1f17e8b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970688"
---
# <a name="get-deviceenrollmentconfiguration"></a><span data-ttu-id="6080b-103">deviceEnrollmentConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="6080b-103">Get deviceEnrollmentConfiguration</span></span>

> <span data-ttu-id="6080b-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6080b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6080b-105">Lesen von Eigenschaften und Beziehungen des [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6080b-105">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6080b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6080b-106">Prerequisites</span></span>
<span data-ttu-id="6080b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6080b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6080b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6080b-109">Permission type</span></span>|<span data-ttu-id="6080b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6080b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6080b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6080b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6080b-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6080b-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6080b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6080b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6080b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6080b-114">Not supported.</span></span>|
|<span data-ttu-id="6080b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6080b-115">Application</span></span>|<span data-ttu-id="6080b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6080b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6080b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6080b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6080b-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6080b-118">Optional query parameters</span></span>
<span data-ttu-id="6080b-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6080b-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6080b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6080b-120">Request headers</span></span>
|<span data-ttu-id="6080b-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6080b-121">Header</span></span>|<span data-ttu-id="6080b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6080b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6080b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6080b-123">Authorization</span></span>|<span data-ttu-id="6080b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6080b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6080b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6080b-125">Accept</span></span>|<span data-ttu-id="6080b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6080b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6080b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6080b-127">Request body</span></span>
<span data-ttu-id="6080b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6080b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6080b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6080b-129">Response</span></span>
<span data-ttu-id="6080b-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6080b-130">If successful, this method returns a `200 OK` response code and [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6080b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6080b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6080b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6080b-132">Request</span></span>
<span data-ttu-id="6080b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6080b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="6080b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6080b-134">Response</span></span>
<span data-ttu-id="6080b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6080b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 392

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
    "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
    "displayName": "Display Name value",
    "description": "Description value",
    "priority": 8,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "version": 7
  }
}
```



