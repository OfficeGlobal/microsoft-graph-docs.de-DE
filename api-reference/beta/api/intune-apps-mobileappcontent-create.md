---
title: Erstellen von „mobileAppContent“
description: Diese Methode erstellt ein neues Objekt des Typs mobileAppContent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8904626782e6df7a0fd6f367f0e0878328a07faf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921892"
---
# <a name="create-mobileappcontent"></a><span data-ttu-id="f91f6-103">Erstellen von „mobileAppContent“</span><span class="sxs-lookup"><span data-stu-id="f91f6-103">Create mobileAppContent</span></span>

> <span data-ttu-id="f91f6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f91f6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f91f6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f91f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f91f6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f91f6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f91f6-107">Diese Methode erstellt ein neues Objekt des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="f91f6-107">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f91f6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f91f6-108">Prerequisites</span></span>
<span data-ttu-id="f91f6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f91f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f91f6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f91f6-111">Permission type</span></span>|<span data-ttu-id="f91f6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f91f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f91f6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f91f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f91f6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f91f6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f91f6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f91f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f91f6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f91f6-116">Not supported.</span></span>|
|<span data-ttu-id="f91f6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f91f6-117">Application</span></span>|<span data-ttu-id="f91f6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f91f6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f91f6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f91f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="f91f6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f91f6-120">Request headers</span></span>
|<span data-ttu-id="f91f6-121">Header</span><span class="sxs-lookup"><span data-stu-id="f91f6-121">Header</span></span>|<span data-ttu-id="f91f6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f91f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f91f6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f91f6-123">Authorization</span></span>|<span data-ttu-id="f91f6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f91f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f91f6-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f91f6-125">Accept</span></span>|<span data-ttu-id="f91f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f91f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f91f6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f91f6-127">Request body</span></span>
<span data-ttu-id="f91f6-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mobileAppContent“ an.</span><span class="sxs-lookup"><span data-stu-id="f91f6-128">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="f91f6-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mobileAppContent“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="f91f6-129">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="f91f6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f91f6-130">Property</span></span>|<span data-ttu-id="f91f6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f91f6-131">Type</span></span>|<span data-ttu-id="f91f6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f91f6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f91f6-133">id</span><span class="sxs-lookup"><span data-stu-id="f91f6-133">id</span></span>|<span data-ttu-id="f91f6-134">String</span><span class="sxs-lookup"><span data-stu-id="f91f6-134">String</span></span>|<span data-ttu-id="f91f6-135">Die Version der App-Inhalte</span><span class="sxs-lookup"><span data-stu-id="f91f6-135">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="f91f6-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f91f6-136">Response</span></span>
<span data-ttu-id="f91f6-137">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f91f6-137">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f91f6-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f91f6-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="f91f6-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f91f6-139">Request</span></span>
<span data-ttu-id="f91f6-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f91f6-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="f91f6-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="f91f6-141">Response</span></span>
<span data-ttu-id="f91f6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f91f6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```





