---
title: OfficeClientConfigurationAssignment aktualisieren
description: Aktualisieren Sie die Eigenschaften eines OfficeClientConfigurationAssignment-Objekts.
author: tfitzmac
ms.openlocfilehash: 78b0ae28bc61bc0d8d8c083502c6f6ef2cf7d0fb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343035"
---
# <a name="update-officeclientconfigurationassignment"></a><span data-ttu-id="43988-103">OfficeClientConfigurationAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="43988-103">Update officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="43988-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="43988-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43988-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="43988-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43988-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="43988-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43988-107">Aktualisieren Sie die Eigenschaften eines [OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="43988-107">Update the properties of a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="43988-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="43988-108">Prerequisites</span></span>
<span data-ttu-id="43988-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43988-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43988-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="43988-111">Permission type</span></span>|<span data-ttu-id="43988-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="43988-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43988-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="43988-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43988-114">\*\* Zu erledigen: Bestimmen der Bereiche \*\*</span><span class="sxs-lookup"><span data-stu-id="43988-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="43988-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="43988-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43988-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43988-116">Not supported.</span></span>|
|<span data-ttu-id="43988-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="43988-117">Application</span></span>|<span data-ttu-id="43988-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43988-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43988-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="43988-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="43988-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="43988-120">Request headers</span></span>
|<span data-ttu-id="43988-121">Header</span><span class="sxs-lookup"><span data-stu-id="43988-121">Header</span></span>|<span data-ttu-id="43988-122">Wert</span><span class="sxs-lookup"><span data-stu-id="43988-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43988-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="43988-123">Authorization</span></span>|<span data-ttu-id="43988-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="43988-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43988-125">Accept</span><span class="sxs-lookup"><span data-stu-id="43988-125">Accept</span></span>|<span data-ttu-id="43988-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43988-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43988-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="43988-127">Request body</span></span>
<span data-ttu-id="43988-128">Geben Sie im Textkörper Anforderung für das Objekt [OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="43988-128">In the request body, supply a JSON representation for the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

<span data-ttu-id="43988-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="43988-129">The following table shows the properties that are required when you create the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

|<span data-ttu-id="43988-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="43988-130">Property</span></span>|<span data-ttu-id="43988-131">Typ</span><span class="sxs-lookup"><span data-stu-id="43988-131">Type</span></span>|<span data-ttu-id="43988-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43988-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43988-133">id</span><span class="sxs-lookup"><span data-stu-id="43988-133">id</span></span>|<span data-ttu-id="43988-134">String</span><span class="sxs-lookup"><span data-stu-id="43988-134">String</span></span>|<span data-ttu-id="43988-135">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="43988-135">Not yet documented</span></span>|
|<span data-ttu-id="43988-136">target</span><span class="sxs-lookup"><span data-stu-id="43988-136">target</span></span>|[<span data-ttu-id="43988-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="43988-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="43988-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="43988-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="43988-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="43988-139">Response</span></span>
<span data-ttu-id="43988-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="43988-140">If successful, this method returns a `200 OK` response code and an updated [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43988-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="43988-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="43988-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="43988-142">Request</span></span>
<span data-ttu-id="43988-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="43988-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
Content-type: application/json
Content-length: 98

{
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="43988-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="43988-144">Response</span></span>
<span data-ttu-id="43988-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="43988-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



