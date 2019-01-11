---
title: Erstellen von „mobileAppContent“
description: Diese Methode erstellt ein neues Objekt des Typs mobileAppContent.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c59d06f506dd27a8aa7b4731df94e0bed2c5480f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831199"
---
# <a name="create-mobileappcontent"></a><span data-ttu-id="8b2be-103">Erstellen von „mobileAppContent“</span><span class="sxs-lookup"><span data-stu-id="8b2be-103">Create mobileAppContent</span></span>

> <span data-ttu-id="8b2be-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8b2be-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b2be-105">Diese Methode erstellt ein neues Objekt des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="8b2be-105">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8b2be-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8b2be-106">Prerequisites</span></span>
<span data-ttu-id="8b2be-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b2be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b2be-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8b2be-109">Permission type</span></span>|<span data-ttu-id="8b2be-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8b2be-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b2be-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8b2be-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8b2be-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b2be-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8b2be-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8b2be-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b2be-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b2be-114">Not supported.</span></span>|
|<span data-ttu-id="8b2be-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8b2be-115">Application</span></span>|<span data-ttu-id="8b2be-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b2be-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b2be-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b2be-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="8b2be-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8b2be-118">Request headers</span></span>
|<span data-ttu-id="8b2be-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8b2be-119">Header</span></span>|<span data-ttu-id="8b2be-120">Wert</span><span class="sxs-lookup"><span data-stu-id="8b2be-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b2be-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b2be-121">Authorization</span></span>|<span data-ttu-id="8b2be-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8b2be-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b2be-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8b2be-123">Accept</span></span>|<span data-ttu-id="8b2be-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8b2be-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b2be-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8b2be-125">Request body</span></span>
<span data-ttu-id="8b2be-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mobileAppContent“ an.</span><span class="sxs-lookup"><span data-stu-id="8b2be-126">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="8b2be-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mobileAppContent“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="8b2be-127">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="8b2be-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8b2be-128">Property</span></span>|<span data-ttu-id="8b2be-129">Typ</span><span class="sxs-lookup"><span data-stu-id="8b2be-129">Type</span></span>|<span data-ttu-id="8b2be-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8b2be-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b2be-131">id</span><span class="sxs-lookup"><span data-stu-id="8b2be-131">id</span></span>|<span data-ttu-id="8b2be-132">String</span><span class="sxs-lookup"><span data-stu-id="8b2be-132">String</span></span>|<span data-ttu-id="8b2be-133">Die Version der App-Inhalte</span><span class="sxs-lookup"><span data-stu-id="8b2be-133">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="8b2be-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b2be-134">Response</span></span>
<span data-ttu-id="8b2be-135">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8b2be-135">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b2be-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8b2be-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="8b2be-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b2be-137">Request</span></span>
<span data-ttu-id="8b2be-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8b2be-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="8b2be-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b2be-139">Response</span></span>
<span data-ttu-id="8b2be-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8b2be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```



