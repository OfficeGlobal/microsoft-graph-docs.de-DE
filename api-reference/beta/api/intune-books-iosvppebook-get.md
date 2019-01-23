---
title: iosVppEBook abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs iosVppEBook.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8e2085f3577be40c84cec721958e77ff6d851dc2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414060"
---
# <a name="get-iosvppebook"></a><span data-ttu-id="b4bb6-103">iosVppEBook abrufen</span><span class="sxs-lookup"><span data-stu-id="b4bb6-103">Get iosVppEBook</span></span>

> <span data-ttu-id="b4bb6-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="b4bb6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b4bb6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b4bb6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4bb6-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b4bb6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4bb6-107">Liest die Eigenschaften und Beziehungen von Objekten des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="b4bb6-107">Read properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4bb6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b4bb6-108">Prerequisites</span></span>
<span data-ttu-id="b4bb6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b4bb6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b4bb6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b4bb6-111">Permission type</span></span>|<span data-ttu-id="b4bb6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b4bb6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4bb6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b4bb6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4bb6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4bb6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b4bb6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b4bb6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4bb6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4bb6-116">Not supported.</span></span>|
|<span data-ttu-id="b4bb6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b4bb6-117">Application</span></span>|<span data-ttu-id="b4bb6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4bb6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4bb6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4bb6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b4bb6-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b4bb6-120">Optional query parameters</span></span>
<span data-ttu-id="b4bb6-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b4bb6-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4bb6-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b4bb6-122">Request headers</span></span>
|<span data-ttu-id="b4bb6-123">Header</span><span class="sxs-lookup"><span data-stu-id="b4bb6-123">Header</span></span>|<span data-ttu-id="b4bb6-124">Wert</span><span class="sxs-lookup"><span data-stu-id="b4bb6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4bb6-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b4bb6-125">Authorization</span></span>|<span data-ttu-id="b4bb6-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b4bb6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4bb6-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b4bb6-127">Accept</span></span>|<span data-ttu-id="b4bb6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b4bb6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4bb6-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b4bb6-129">Request body</span></span>
<span data-ttu-id="b4bb6-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b4bb6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4bb6-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4bb6-131">Response</span></span>
<span data-ttu-id="b4bb6-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [iosVppEBook](../resources/intune-books-iosvppebook.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b4bb6-132">If successful, this method returns a `200 OK` response code and [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4bb6-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b4bb6-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4bb6-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4bb6-134">Request</span></span>
<span data-ttu-id="b4bb6-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b4bb6-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}
```

### <a name="response"></a><span data-ttu-id="b4bb6-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4bb6-136">Response</span></span>
<span data-ttu-id="b4bb6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b4bb6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1101

{
  "value": {
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
}
```




