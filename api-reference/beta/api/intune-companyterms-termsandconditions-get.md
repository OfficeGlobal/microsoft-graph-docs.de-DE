---
title: termsAndConditions abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs termsAndConditions.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9839d5fb2cf91848d066bdb7a426ec33c283742c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975805"
---
# <a name="get-termsandconditions"></a><span data-ttu-id="c3c28-103">termsAndConditions abrufen</span><span class="sxs-lookup"><span data-stu-id="c3c28-103">Get termsAndConditions</span></span>

> <span data-ttu-id="c3c28-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c3c28-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3c28-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c3c28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3c28-106">Liest die Eigenschaften und Beziehungen von Objekten des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="c3c28-106">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3c28-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c3c28-107">Prerequisites</span></span>
<span data-ttu-id="c3c28-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3c28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3c28-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c3c28-110">Permission type</span></span>|<span data-ttu-id="c3c28-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c3c28-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3c28-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c3c28-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3c28-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3c28-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c3c28-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c3c28-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3c28-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c3c28-115">Not supported.</span></span>|
|<span data-ttu-id="c3c28-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c3c28-116">Application</span></span>|<span data-ttu-id="c3c28-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c3c28-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3c28-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c3c28-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c3c28-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c3c28-119">Optional query parameters</span></span>
<span data-ttu-id="c3c28-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c3c28-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3c28-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c3c28-121">Request headers</span></span>
|<span data-ttu-id="c3c28-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c3c28-122">Header</span></span>|<span data-ttu-id="c3c28-123">Wert</span><span class="sxs-lookup"><span data-stu-id="c3c28-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3c28-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3c28-124">Authorization</span></span>|<span data-ttu-id="c3c28-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c3c28-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3c28-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c3c28-126">Accept</span></span>|<span data-ttu-id="c3c28-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c3c28-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3c28-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c3c28-128">Request body</span></span>
<span data-ttu-id="c3c28-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c3c28-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3c28-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="c3c28-130">Response</span></span>
<span data-ttu-id="c3c28-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c3c28-131">If successful, this method returns a `200 OK` response code and [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3c28-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c3c28-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3c28-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c3c28-133">Request</span></span>
<span data-ttu-id="c3c28-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c3c28-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
```

### <a name="response"></a><span data-ttu-id="c3c28-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="c3c28-135">Response</span></span>
<span data-ttu-id="c3c28-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c3c28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 546

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditions",
    "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "description": "Description value",
    "title": "Title value",
    "bodyText": "Body Text value",
    "acceptanceStatement": "Acceptance Statement value",
    "version": 7
  }
}
```




