---
title: Auflisten von „windows10SecureAssessmentConfiguration“
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs windows10SecureAssessmentConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c532bc3c1c1b876459b6f4d6bb96e7a18137515
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976561"
---
# <a name="list-windows10secureassessmentconfigurations"></a><span data-ttu-id="84e87-103">Auflisten von „windows10SecureAssessmentConfiguration“</span><span class="sxs-lookup"><span data-stu-id="84e87-103">List windows10SecureAssessmentConfigurations</span></span>

> <span data-ttu-id="84e87-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="84e87-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84e87-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="84e87-105">List properties and relationships of the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84e87-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="84e87-106">Prerequisites</span></span>
<span data-ttu-id="84e87-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84e87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84e87-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="84e87-109">Permission type</span></span>|<span data-ttu-id="84e87-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="84e87-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84e87-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="84e87-111">Delegated (work or school account)</span></span>|<span data-ttu-id="84e87-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="84e87-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="84e87-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="84e87-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84e87-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84e87-114">Not supported.</span></span>|
|<span data-ttu-id="84e87-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="84e87-115">Application</span></span>|<span data-ttu-id="84e87-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84e87-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84e87-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="84e87-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="84e87-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="84e87-118">Request headers</span></span>
|<span data-ttu-id="84e87-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="84e87-119">Header</span></span>|<span data-ttu-id="84e87-120">Wert</span><span class="sxs-lookup"><span data-stu-id="84e87-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84e87-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="84e87-121">Authorization</span></span>|<span data-ttu-id="84e87-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="84e87-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84e87-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="84e87-123">Accept</span></span>|<span data-ttu-id="84e87-124">application/json</span><span class="sxs-lookup"><span data-stu-id="84e87-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84e87-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="84e87-125">Request body</span></span>
<span data-ttu-id="84e87-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="84e87-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84e87-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="84e87-127">Response</span></span>
<span data-ttu-id="84e87-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="84e87-128">If successful, this method returns a `200 OK` response code and a collection of [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84e87-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="84e87-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="84e87-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="84e87-130">Request</span></span>
<span data-ttu-id="84e87-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="84e87-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="84e87-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="84e87-132">Response</span></span>
<span data-ttu-id="84e87-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="84e87-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 612

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
      "id": "f60d71be-71be-f60d-be71-0df6be710df6",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "launchUri": "Launch Uri value",
      "configurationAccount": "Configuration Account value",
      "allowPrinting": true,
      "allowScreenCapture": true,
      "allowTextSuggestion": true
    }
  ]
}
```



