---
title: Abrufen von „termsAndConditionsAcceptanceStatus“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs termsAndConditionsAcceptanceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 055becaff4148cf27dbb978eab6713b2c996cb18
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163798"
---
# <a name="get-termsandconditionsacceptancestatus"></a><span data-ttu-id="f48fb-103">Abrufen von „termsAndConditionsAcceptanceStatus“</span><span class="sxs-lookup"><span data-stu-id="f48fb-103">Get termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="f48fb-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f48fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f48fb-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f48fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f48fb-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="f48fb-106">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f48fb-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f48fb-107">Prerequisites</span></span>
<span data-ttu-id="f48fb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f48fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f48fb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f48fb-110">Permission type</span></span>|<span data-ttu-id="f48fb-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f48fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f48fb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f48fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f48fb-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f48fb-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f48fb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f48fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f48fb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f48fb-115">Not supported.</span></span>|
|<span data-ttu-id="f48fb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f48fb-116">Application</span></span>|<span data-ttu-id="f48fb-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f48fb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f48fb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f48fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f48fb-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f48fb-119">Optional query parameters</span></span>
<span data-ttu-id="f48fb-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f48fb-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f48fb-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f48fb-121">Request headers</span></span>
|<span data-ttu-id="f48fb-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f48fb-122">Header</span></span>|<span data-ttu-id="f48fb-123">Wert</span><span class="sxs-lookup"><span data-stu-id="f48fb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f48fb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f48fb-124">Authorization</span></span>|<span data-ttu-id="f48fb-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f48fb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f48fb-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f48fb-126">Accept</span></span>|<span data-ttu-id="f48fb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f48fb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f48fb-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f48fb-128">Request body</span></span>
<span data-ttu-id="f48fb-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f48fb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f48fb-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="f48fb-130">Response</span></span>
<span data-ttu-id="f48fb-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f48fb-131">If successful, this method returns a `200 OK` response code and [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f48fb-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f48fb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f48fb-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f48fb-133">Request</span></span>
<span data-ttu-id="f48fb-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f48fb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

### <a name="response"></a><span data-ttu-id="f48fb-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="f48fb-135">Response</span></span>
<span data-ttu-id="f48fb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f48fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 289

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
    "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
    "userDisplayName": "User Display Name value",
    "acceptedVersion": 15,
    "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
  }
}
```




