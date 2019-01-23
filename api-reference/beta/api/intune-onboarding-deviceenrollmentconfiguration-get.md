---
title: deviceEnrollmentConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceEnrollmentConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 10c202369ff6c129f6a2b66c625fd055ddba40b2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414452"
---
# <a name="get-deviceenrollmentconfiguration"></a><span data-ttu-id="78050-103">deviceEnrollmentConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="78050-103">Get deviceEnrollmentConfiguration</span></span>

> <span data-ttu-id="78050-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="78050-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="78050-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="78050-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78050-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="78050-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78050-107">Lesen von Eigenschaften und Beziehungen des [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="78050-107">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78050-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="78050-108">Prerequisites</span></span>
<span data-ttu-id="78050-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="78050-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="78050-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="78050-111">Permission type</span></span>|<span data-ttu-id="78050-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="78050-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78050-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="78050-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78050-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="78050-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="78050-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="78050-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78050-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="78050-116">Not supported.</span></span>|
|<span data-ttu-id="78050-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="78050-117">Application</span></span>|<span data-ttu-id="78050-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="78050-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78050-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="78050-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="78050-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="78050-120">Optional query parameters</span></span>
<span data-ttu-id="78050-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="78050-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="78050-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="78050-122">Request headers</span></span>
|<span data-ttu-id="78050-123">Header</span><span class="sxs-lookup"><span data-stu-id="78050-123">Header</span></span>|<span data-ttu-id="78050-124">Wert</span><span class="sxs-lookup"><span data-stu-id="78050-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78050-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="78050-125">Authorization</span></span>|<span data-ttu-id="78050-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="78050-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78050-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="78050-127">Accept</span></span>|<span data-ttu-id="78050-128">application/json</span><span class="sxs-lookup"><span data-stu-id="78050-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78050-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="78050-129">Request body</span></span>
<span data-ttu-id="78050-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="78050-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78050-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="78050-131">Response</span></span>
<span data-ttu-id="78050-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="78050-132">If successful, this method returns a `200 OK` response code and [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78050-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="78050-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="78050-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="78050-134">Request</span></span>
<span data-ttu-id="78050-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="78050-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="78050-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="78050-136">Response</span></span>
<span data-ttu-id="78050-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="78050-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




