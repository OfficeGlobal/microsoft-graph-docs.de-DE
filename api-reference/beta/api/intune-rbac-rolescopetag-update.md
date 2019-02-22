---
title: RoleScopeTag aktualisieren
description: Aktualisieren der Eigenschaften eines roleScopeTag-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b6616c7b847f260cb1fba86561387d33aaaaa438
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145521"
---
# <a name="update-rolescopetag"></a><span data-ttu-id="e4af6-103">RoleScopeTag aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e4af6-103">Update roleScopeTag</span></span>

> <span data-ttu-id="e4af6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e4af6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4af6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e4af6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4af6-106">Aktualisieren der Eigenschaften eines [roleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e4af6-106">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4af6-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e4af6-107">Prerequisites</span></span>
<span data-ttu-id="e4af6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e4af6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e4af6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e4af6-110">Permission type</span></span>|<span data-ttu-id="e4af6-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e4af6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4af6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e4af6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4af6-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4af6-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="e4af6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e4af6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4af6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4af6-115">Not supported.</span></span>|
|<span data-ttu-id="e4af6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e4af6-116">Application</span></span>|<span data-ttu-id="e4af6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4af6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4af6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4af6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleScopeTags/{roleScopeTagId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="request-headers"></a><span data-ttu-id="e4af6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e4af6-119">Request headers</span></span>
|<span data-ttu-id="e4af6-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e4af6-120">Header</span></span>|<span data-ttu-id="e4af6-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e4af6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4af6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4af6-122">Authorization</span></span>|<span data-ttu-id="e4af6-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e4af6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4af6-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e4af6-124">Accept</span></span>|<span data-ttu-id="e4af6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e4af6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4af6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e4af6-126">Request body</span></span>
<span data-ttu-id="e4af6-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [roleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="e4af6-127">In the request body, supply a JSON representation for the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

<span data-ttu-id="e4af6-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [roleScopeTag](../resources/intune-rbac-rolescopetag.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e4af6-128">The following table shows the properties that are required when you create the [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>

|<span data-ttu-id="e4af6-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e4af6-129">Property</span></span>|<span data-ttu-id="e4af6-130">Typ</span><span class="sxs-lookup"><span data-stu-id="e4af6-130">Type</span></span>|<span data-ttu-id="e4af6-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4af6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4af6-132">id</span><span class="sxs-lookup"><span data-stu-id="e4af6-132">id</span></span>|<span data-ttu-id="e4af6-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4af6-133">String</span></span>|<span data-ttu-id="e4af6-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e4af6-134">Key of the entity.</span></span> <span data-ttu-id="e4af6-135">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="e4af6-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="e4af6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e4af6-136">displayName</span></span>|<span data-ttu-id="e4af6-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4af6-137">String</span></span>|<span data-ttu-id="e4af6-138">Die Anzeige oder der angezeigte Name des Rollenbereichs Tags.</span><span class="sxs-lookup"><span data-stu-id="e4af6-138">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="e4af6-139">description</span><span class="sxs-lookup"><span data-stu-id="e4af6-139">description</span></span>|<span data-ttu-id="e4af6-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4af6-140">String</span></span>|<span data-ttu-id="e4af6-141">Beschreibung des Rollenbereichs Tags.</span><span class="sxs-lookup"><span data-stu-id="e4af6-141">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="e4af6-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4af6-142">Response</span></span>
<span data-ttu-id="e4af6-143">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [roleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e4af6-143">If successful, this method returns a `200 OK` response code and an updated [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4af6-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e4af6-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4af6-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4af6-145">Request</span></span>
<span data-ttu-id="e4af6-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e4af6-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}
Content-type: application/json
Content-length: 133

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="e4af6-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4af6-147">Response</span></span>
<span data-ttu-id="e4af6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4af6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 182

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
  "displayName": "Display Name value",
  "description": "Description value"
}
```




