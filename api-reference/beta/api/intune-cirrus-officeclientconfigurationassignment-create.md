---
title: OfficeClientConfigurationAssignment erstellen
description: Hinzufügen einer Zielgruppe zu einer vorhandenen Richtlinie
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e646b70ea3e18a79aaee5b4129e54da833c5c4a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155265"
---
# <a name="create-officeclientconfigurationassignment"></a><span data-ttu-id="ebbab-103">OfficeClientConfigurationAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="ebbab-103">Create officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="ebbab-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ebbab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebbab-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ebbab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebbab-106">Hinzufügen einer Zielgruppe zu einer vorhandenen Richtlinie</span><span class="sxs-lookup"><span data-stu-id="ebbab-106">Add a target group to an existing policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebbab-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ebbab-107">Prerequisites</span></span>
<span data-ttu-id="ebbab-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebbab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebbab-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ebbab-110">Permission type</span></span>|<span data-ttu-id="ebbab-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ebbab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebbab-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ebbab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ebbab-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebbab-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ebbab-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ebbab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebbab-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ebbab-115">Not supported.</span></span>|
|<span data-ttu-id="ebbab-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ebbab-116">Application</span></span>|<span data-ttu-id="ebbab-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ebbab-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebbab-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ebbab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{key}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ebbab-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ebbab-119">Request headers</span></span>
|<span data-ttu-id="ebbab-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ebbab-120">Header</span></span>|<span data-ttu-id="ebbab-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ebbab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebbab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebbab-122">Authorization</span></span>|<span data-ttu-id="ebbab-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ebbab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebbab-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ebbab-124">Accept</span></span>|<span data-ttu-id="ebbab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ebbab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebbab-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ebbab-126">Request body</span></span>
<span data-ttu-id="ebbab-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das officeClientConfigurationAssignment-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="ebbab-127">In the request body, supply a JSON representation for the officeClientConfigurationAssignment object.</span></span>

<span data-ttu-id="ebbab-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der officeClientConfigurationAssignment erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ebbab-128">The following table shows the properties that are required when you create the officeClientConfigurationAssignment.</span></span>

|<span data-ttu-id="ebbab-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ebbab-129">Property</span></span>|<span data-ttu-id="ebbab-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ebbab-130">Type</span></span>|<span data-ttu-id="ebbab-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ebbab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebbab-132">id</span><span class="sxs-lookup"><span data-stu-id="ebbab-132">id</span></span>|<span data-ttu-id="ebbab-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ebbab-133">String</span></span>|<span data-ttu-id="ebbab-134">ID des OfficeConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="ebbab-134">Id of the OfficeConfigurationAssignment.</span></span>|
|<span data-ttu-id="ebbab-135">target</span><span class="sxs-lookup"><span data-stu-id="ebbab-135">target</span></span>|[<span data-ttu-id="ebbab-136">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ebbab-136">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="ebbab-137">Die vom Administrator definierte Zielzuweisung.</span><span class="sxs-lookup"><span data-stu-id="ebbab-137">The target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="ebbab-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="ebbab-138">Response</span></span>
<span data-ttu-id="ebbab-139">Bei erfolgreicher Ausführung gibt diese Methode den `200 Created` Antwortcode und ein [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ebbab-139">If successful, this method returns a `200 Created` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebbab-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ebbab-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebbab-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ebbab-141">Request</span></span>
<span data-ttu-id="ebbab-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ebbab-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="ebbab-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="ebbab-143">Response</span></span>
<span data-ttu-id="ebbab-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ebbab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "804730f3-30f3-8047-f330-4780f3304780",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```



