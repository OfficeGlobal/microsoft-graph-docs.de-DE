---
title: Abrufen von „notificationMessageTemplate“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs notificationMessageTemplate.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f30bf3b54070f7a8ab37745639f58d16f6a99aa2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884035"
---
# <a name="get-notificationmessagetemplate"></a><span data-ttu-id="d7acf-103">Abrufen von „notificationMessageTemplate“</span><span class="sxs-lookup"><span data-stu-id="d7acf-103">Get notificationMessageTemplate</span></span>

> <span data-ttu-id="d7acf-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d7acf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7acf-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="d7acf-105">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d7acf-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d7acf-106">Prerequisites</span></span>
<span data-ttu-id="d7acf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7acf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7acf-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d7acf-109">Permission type</span></span>|<span data-ttu-id="d7acf-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d7acf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7acf-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d7acf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d7acf-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7acf-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d7acf-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d7acf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7acf-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7acf-114">Not supported.</span></span>|
|<span data-ttu-id="d7acf-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d7acf-115">Application</span></span>|<span data-ttu-id="d7acf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7acf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7acf-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7acf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d7acf-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d7acf-118">Optional query parameters</span></span>
<span data-ttu-id="d7acf-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d7acf-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d7acf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d7acf-120">Request headers</span></span>
|<span data-ttu-id="d7acf-121">Header</span><span class="sxs-lookup"><span data-stu-id="d7acf-121">Header</span></span>|<span data-ttu-id="d7acf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d7acf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7acf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7acf-123">Authorization</span></span>|<span data-ttu-id="d7acf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d7acf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7acf-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d7acf-125">Accept</span></span>|<span data-ttu-id="d7acf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d7acf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7acf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d7acf-127">Request body</span></span>
<span data-ttu-id="d7acf-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d7acf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7acf-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7acf-129">Response</span></span>
<span data-ttu-id="d7acf-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d7acf-130">If successful, this method returns a `200 OK` response code and [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7acf-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d7acf-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d7acf-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7acf-132">Request</span></span>
<span data-ttu-id="d7acf-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d7acf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

### <a name="response"></a><span data-ttu-id="d7acf-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7acf-134">Response</span></span>
<span data-ttu-id="d7acf-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d7acf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 341

{
  "value": {
    "@odata.type": "#microsoft.graph.notificationMessageTemplate",
    "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "defaultLocale": "Default Locale value",
    "brandingOptions": "includeCompanyLogo"
  }
}
```



