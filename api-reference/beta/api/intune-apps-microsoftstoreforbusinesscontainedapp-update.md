---
title: MicrosoftStoreForBusinessContainedApp aktualisieren
description: Aktualisieren der Eigenschaften eines microsoftStoreForBusinessContainedApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4eb65cec330fb8027bbbb6158dc31ee17444b060
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146480"
---
# <a name="update-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="d7fea-103">MicrosoftStoreForBusinessContainedApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d7fea-103">Update microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="d7fea-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d7fea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7fea-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d7fea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7fea-106">Aktualisieren der Eigenschaften eines [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d7fea-106">Update the properties of a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7fea-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d7fea-107">Prerequisites</span></span>
<span data-ttu-id="d7fea-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d7fea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d7fea-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d7fea-110">Permission type</span></span>|<span data-ttu-id="d7fea-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d7fea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7fea-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d7fea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7fea-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7fea-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d7fea-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d7fea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7fea-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7fea-115">Not supported.</span></span>|
|<span data-ttu-id="d7fea-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d7fea-116">Application</span></span>|<span data-ttu-id="d7fea-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7fea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7fea-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7fea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="d7fea-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d7fea-119">Request headers</span></span>
|<span data-ttu-id="d7fea-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d7fea-120">Header</span></span>|<span data-ttu-id="d7fea-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d7fea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7fea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7fea-122">Authorization</span></span>|<span data-ttu-id="d7fea-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d7fea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7fea-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d7fea-124">Accept</span></span>|<span data-ttu-id="d7fea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7fea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7fea-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d7fea-126">Request body</span></span>
<span data-ttu-id="d7fea-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="d7fea-127">In the request body, supply a JSON representation for the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

<span data-ttu-id="d7fea-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d7fea-128">The following table shows the properties that are required when you create the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span></span>

|<span data-ttu-id="d7fea-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d7fea-129">Property</span></span>|<span data-ttu-id="d7fea-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d7fea-130">Type</span></span>|<span data-ttu-id="d7fea-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7fea-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7fea-132">id</span><span class="sxs-lookup"><span data-stu-id="d7fea-132">id</span></span>|<span data-ttu-id="d7fea-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d7fea-133">String</span></span>|<span data-ttu-id="d7fea-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d7fea-134">Key of the entity.</span></span> <span data-ttu-id="d7fea-135">Geerbt von [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7fea-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="d7fea-136">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="d7fea-136">appUserModelId</span></span>|<span data-ttu-id="d7fea-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d7fea-137">String</span></span>|<span data-ttu-id="d7fea-138">Die APP-Benutzermodell-ID der enthaltenen App eines MicrosoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="d7fea-138">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="d7fea-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7fea-139">Response</span></span>
<span data-ttu-id="d7fea-140">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d7fea-140">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7fea-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d7fea-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7fea-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7fea-142">Request</span></span>
<span data-ttu-id="d7fea-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d7fea-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="d7fea-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7fea-144">Response</span></span>
<span data-ttu-id="d7fea-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d7fea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 176

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "id": "bf1d79df-79df-bf1d-df79-1dbfdf791dbf",
  "appUserModelId": "App User Model Id value"
}
```




