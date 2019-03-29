---
title: WindowsManagementApp aktualisieren
description: Aktualisieren der Eigenschaften eines windowsManagementApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b68af1276d24845e3bb90b5e7a6db38a09806aa
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962841"
---
# <a name="update-windowsmanagementapp"></a><span data-ttu-id="958e8-103">WindowsManagementApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="958e8-103">Update windowsManagementApp</span></span>

> <span data-ttu-id="958e8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="958e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="958e8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="958e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="958e8-106">Aktualisieren der Eigenschaften eines [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="958e8-106">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="958e8-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="958e8-107">Prerequisites</span></span>
<span data-ttu-id="958e8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="958e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="958e8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="958e8-110">Permission type</span></span>|<span data-ttu-id="958e8-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="958e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="958e8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="958e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="958e8-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="958e8-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="958e8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="958e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="958e8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="958e8-115">Not supported.</span></span>|
|<span data-ttu-id="958e8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="958e8-116">Application</span></span>|<span data-ttu-id="958e8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="958e8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="958e8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="958e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a><span data-ttu-id="958e8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="958e8-119">Request headers</span></span>
|<span data-ttu-id="958e8-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="958e8-120">Header</span></span>|<span data-ttu-id="958e8-121">Wert</span><span class="sxs-lookup"><span data-stu-id="958e8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="958e8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="958e8-122">Authorization</span></span>|<span data-ttu-id="958e8-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="958e8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="958e8-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="958e8-124">Accept</span></span>|<span data-ttu-id="958e8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="958e8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="958e8-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="958e8-126">Request body</span></span>
<span data-ttu-id="958e8-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="958e8-127">In the request body, supply a JSON representation for the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

<span data-ttu-id="958e8-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="958e8-128">The following table shows the properties that are required when you create the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span></span>

|<span data-ttu-id="958e8-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="958e8-129">Property</span></span>|<span data-ttu-id="958e8-130">Typ</span><span class="sxs-lookup"><span data-stu-id="958e8-130">Type</span></span>|<span data-ttu-id="958e8-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="958e8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="958e8-132">id</span><span class="sxs-lookup"><span data-stu-id="958e8-132">id</span></span>|<span data-ttu-id="958e8-133">String</span><span class="sxs-lookup"><span data-stu-id="958e8-133">String</span></span>|<span data-ttu-id="958e8-134">Eindeutige ID für die Windows-Verwaltungs-App</span><span class="sxs-lookup"><span data-stu-id="958e8-134">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="958e8-135">availableVersion</span><span class="sxs-lookup"><span data-stu-id="958e8-135">availableVersion</span></span>|<span data-ttu-id="958e8-136">String</span><span class="sxs-lookup"><span data-stu-id="958e8-136">String</span></span>|<span data-ttu-id="958e8-137">Verfügbare Version der Windows-Verwaltungs-app.</span><span class="sxs-lookup"><span data-stu-id="958e8-137">Windows management app available version.</span></span>|



## <a name="response"></a><span data-ttu-id="958e8-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="958e8-138">Response</span></span>
<span data-ttu-id="958e8-139">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="958e8-139">If successful, this method returns a `200 OK` response code and an updated [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="958e8-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="958e8-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="958e8-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="958e8-141">Request</span></span>
<span data-ttu-id="958e8-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="958e8-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 112

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "availableVersion": "Available Version value"
}
```

### <a name="response"></a><span data-ttu-id="958e8-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="958e8-143">Response</span></span>
<span data-ttu-id="958e8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="958e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 161

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "5facc79c-c79c-5fac-9cc7-ac5f9cc7ac5f",
  "availableVersion": "Available Version value"
}
```




