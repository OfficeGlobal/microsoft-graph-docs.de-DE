---
title: Auflisten von „iosVppEBook“
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs iosVppEBook auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ff43f2f398a4e89e37821867634c690d559ee67
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150666"
---
# <a name="list-iosvppebooks"></a><span data-ttu-id="a3431-103">Auflisten von „iosVppEBook“</span><span class="sxs-lookup"><span data-stu-id="a3431-103">List iosVppEBooks</span></span>

> <span data-ttu-id="a3431-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a3431-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3431-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a3431-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3431-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md) auf.</span><span class="sxs-lookup"><span data-stu-id="a3431-106">List properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3431-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a3431-107">Prerequisites</span></span>
<span data-ttu-id="a3431-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a3431-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a3431-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a3431-110">Permission type</span></span>|<span data-ttu-id="a3431-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a3431-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3431-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a3431-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3431-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3431-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a3431-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a3431-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3431-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a3431-115">Not supported.</span></span>|
|<span data-ttu-id="a3431-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a3431-116">Application</span></span>|<span data-ttu-id="a3431-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a3431-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3431-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3431-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="a3431-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a3431-119">Request headers</span></span>
|<span data-ttu-id="a3431-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a3431-120">Header</span></span>|<span data-ttu-id="a3431-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a3431-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3431-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3431-122">Authorization</span></span>|<span data-ttu-id="a3431-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a3431-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3431-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a3431-124">Accept</span></span>|<span data-ttu-id="a3431-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a3431-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3431-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a3431-126">Request body</span></span>
<span data-ttu-id="a3431-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a3431-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3431-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3431-128">Response</span></span>
<span data-ttu-id="a3431-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a3431-129">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBook](../resources/intune-books-iosvppebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3431-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a3431-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3431-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3431-131">Request</span></span>
<span data-ttu-id="a3431-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a3431-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="a3431-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3431-133">Response</span></span>
<span data-ttu-id="a3431-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a3431-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1171

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppEBook",
      "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
      "largeCover": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "informationUrl": "https://example.com/informationUrl/",
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
      "appleId": "Apple Id value",
      "vppOrganizationName": "Vpp Organization Name value",
      "genres": [
        "Genres value"
      ],
      "language": "Language value",
      "seller": "Seller value",
      "totalLicenseCount": 1,
      "usedLicenseCount": 0,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




