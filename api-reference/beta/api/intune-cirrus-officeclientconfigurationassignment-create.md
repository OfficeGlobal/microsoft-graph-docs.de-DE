---
title: Erstellen von officeClientConfigurationAssignment
description: Hinzufügen einer Zielgruppe zu einer vorhandenen Richtlinie.
author: tfitzmac
ms.openlocfilehash: 850f82f005f46e15a598dd0e08043cca66ffe6bf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324836"
---
# <a name="create-officeclientconfigurationassignment"></a><span data-ttu-id="1da46-103">Erstellen von officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1da46-103">Create officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="1da46-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1da46-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1da46-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1da46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1da46-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1da46-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1da46-107">Hinzufügen einer Zielgruppe zu einer vorhandenen Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="1da46-107">Add a target group to an existing policy.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1da46-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1da46-108">Prerequisites</span></span>
<span data-ttu-id="1da46-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1da46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1da46-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1da46-111">Permission type</span></span>|<span data-ttu-id="1da46-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1da46-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1da46-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1da46-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1da46-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1da46-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1da46-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1da46-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1da46-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1da46-116">Not supported.</span></span>|
|<span data-ttu-id="1da46-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1da46-117">Application</span></span>|<span data-ttu-id="1da46-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1da46-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1da46-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1da46-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{key}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1da46-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1da46-120">Request headers</span></span>
|<span data-ttu-id="1da46-121">Header</span><span class="sxs-lookup"><span data-stu-id="1da46-121">Header</span></span>|<span data-ttu-id="1da46-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1da46-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1da46-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1da46-123">Authorization</span></span>|<span data-ttu-id="1da46-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1da46-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1da46-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1da46-125">Accept</span></span>|<span data-ttu-id="1da46-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1da46-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1da46-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1da46-127">Request body</span></span>
<span data-ttu-id="1da46-128">Geben Sie im Textkörper Anforderung für das Objekt OfficeClientConfigurationAssignment eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="1da46-128">In the request body, supply a JSON representation for the officeClientConfigurationAssignment object.</span></span>

<span data-ttu-id="1da46-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die OfficeClientConfigurationAssignment erstellen.</span><span class="sxs-lookup"><span data-stu-id="1da46-129">The following table shows the properties that are required when you create the officeClientConfigurationAssignment.</span></span>

|<span data-ttu-id="1da46-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1da46-130">Property</span></span>|<span data-ttu-id="1da46-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1da46-131">Type</span></span>|<span data-ttu-id="1da46-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1da46-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1da46-133">id</span><span class="sxs-lookup"><span data-stu-id="1da46-133">id</span></span>|<span data-ttu-id="1da46-134">String</span><span class="sxs-lookup"><span data-stu-id="1da46-134">String</span></span>|<span data-ttu-id="1da46-135">ID des der OfficeConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="1da46-135">Id of the OfficeConfigurationAssignment.</span></span>|
|<span data-ttu-id="1da46-136">target</span><span class="sxs-lookup"><span data-stu-id="1da46-136">target</span></span>|[<span data-ttu-id="1da46-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1da46-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="1da46-138">Die Ziel-Zuordnung, die durch den Administrator definiert</span><span class="sxs-lookup"><span data-stu-id="1da46-138">The target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="1da46-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="1da46-139">Response</span></span>
<span data-ttu-id="1da46-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 Created` Antwortcode und eines [OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1da46-140">If successful, this method returns a `200 Created` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1da46-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1da46-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="1da46-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1da46-142">Request</span></span>
<span data-ttu-id="1da46-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1da46-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1da46-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="1da46-144">Response</span></span>
<span data-ttu-id="1da46-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1da46-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



