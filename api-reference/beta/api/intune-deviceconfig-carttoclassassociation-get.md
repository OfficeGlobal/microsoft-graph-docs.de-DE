---
title: CartToClassAssociation abrufen
description: Lesen von Eigenschaften und Beziehungen des cartToClassAssociation-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c093bb291acec10c76b39f2e99bb4383c91b7ef
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170322"
---
# <a name="get-carttoclassassociation"></a><span data-ttu-id="3fe6f-103">CartToClassAssociation abrufen</span><span class="sxs-lookup"><span data-stu-id="3fe6f-103">Get cartToClassAssociation</span></span>

> <span data-ttu-id="3fe6f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3fe6f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3fe6f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3fe6f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fe6f-106">Lesen von Eigenschaften und Beziehungen des [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3fe6f-106">Read properties and relationships of the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fe6f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3fe6f-107">Prerequisites</span></span>
<span data-ttu-id="3fe6f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3fe6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3fe6f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3fe6f-110">Permission type</span></span>|<span data-ttu-id="3fe6f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3fe6f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fe6f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3fe6f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3fe6f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fe6f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3fe6f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3fe6f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fe6f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3fe6f-115">Not supported.</span></span>|
|<span data-ttu-id="3fe6f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3fe6f-116">Application</span></span>|<span data-ttu-id="3fe6f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3fe6f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fe6f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3fe6f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3fe6f-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3fe6f-119">Optional query parameters</span></span>
<span data-ttu-id="3fe6f-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3fe6f-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3fe6f-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3fe6f-121">Request headers</span></span>
|<span data-ttu-id="3fe6f-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3fe6f-122">Header</span></span>|<span data-ttu-id="3fe6f-123">Wert</span><span class="sxs-lookup"><span data-stu-id="3fe6f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fe6f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fe6f-124">Authorization</span></span>|<span data-ttu-id="3fe6f-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3fe6f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fe6f-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3fe6f-126">Accept</span></span>|<span data-ttu-id="3fe6f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3fe6f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fe6f-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3fe6f-128">Request body</span></span>
<span data-ttu-id="3fe6f-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3fe6f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fe6f-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="3fe6f-130">Response</span></span>
<span data-ttu-id="3fe6f-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3fe6f-131">If successful, this method returns a `200 OK` response code and [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fe6f-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3fe6f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fe6f-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3fe6f-133">Request</span></span>
<span data-ttu-id="3fe6f-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3fe6f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

### <a name="response"></a><span data-ttu-id="3fe6f-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="3fe6f-135">Response</span></span>
<span data-ttu-id="3fe6f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3fe6f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 488

{
  "value": {
    "@odata.type": "#microsoft.graph.cartToClassAssociation",
    "id": "9bdc58dd-58dd-9bdc-dd58-dc9bdd58dc9b",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "version": 7,
    "displayName": "Display Name value",
    "description": "Description value",
    "deviceCartIds": [
      "Device Cart Ids value"
    ],
    "classroomIds": [
      "Classroom Ids value"
    ]
  }
}
```




