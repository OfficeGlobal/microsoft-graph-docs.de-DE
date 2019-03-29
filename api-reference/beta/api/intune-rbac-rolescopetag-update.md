---
title: RoleScopeTag aktualisieren
description: Aktualisieren der Eigenschaften eines roleScopeTag-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a0adb3e151eb4b9d54a7c83d886deb99ac23573
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959425"
---
# <a name="update-rolescopetag"></a><span data-ttu-id="0d30a-103">RoleScopeTag aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0d30a-103">Update roleScopeTag</span></span>

> <span data-ttu-id="0d30a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0d30a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d30a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0d30a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d30a-106">Aktualisieren der Eigenschaften eines [roleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0d30a-106">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d30a-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0d30a-107">Prerequisites</span></span>
<span data-ttu-id="0d30a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d30a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d30a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0d30a-110">Permission type</span></span>|<span data-ttu-id="0d30a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0d30a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d30a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0d30a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0d30a-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d30a-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="0d30a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0d30a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d30a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d30a-115">Not supported.</span></span>|
|<span data-ttu-id="0d30a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0d30a-116">Application</span></span>|<span data-ttu-id="0d30a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d30a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d30a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d30a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleScopeTags/{roleScopeTagId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="request-headers"></a><span data-ttu-id="0d30a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0d30a-119">Request headers</span></span>
|<span data-ttu-id="0d30a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0d30a-120">Header</span></span>|<span data-ttu-id="0d30a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="0d30a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d30a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d30a-122">Authorization</span></span>|<span data-ttu-id="0d30a-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0d30a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d30a-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0d30a-124">Accept</span></span>|<span data-ttu-id="0d30a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0d30a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d30a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0d30a-126">Request body</span></span>
<span data-ttu-id="0d30a-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [roleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="0d30a-127">In the request body, supply a JSON representation for the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

<span data-ttu-id="0d30a-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [roleScopeTag](../resources/intune-rbac-rolescopetag.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0d30a-128">The following table shows the properties that are required when you create the [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>

|<span data-ttu-id="0d30a-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0d30a-129">Property</span></span>|<span data-ttu-id="0d30a-130">Typ</span><span class="sxs-lookup"><span data-stu-id="0d30a-130">Type</span></span>|<span data-ttu-id="0d30a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d30a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d30a-132">id</span><span class="sxs-lookup"><span data-stu-id="0d30a-132">id</span></span>|<span data-ttu-id="0d30a-133">String</span><span class="sxs-lookup"><span data-stu-id="0d30a-133">String</span></span>|<span data-ttu-id="0d30a-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0d30a-134">Key of the entity.</span></span> <span data-ttu-id="0d30a-135">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="0d30a-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="0d30a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0d30a-136">displayName</span></span>|<span data-ttu-id="0d30a-137">String</span><span class="sxs-lookup"><span data-stu-id="0d30a-137">String</span></span>|<span data-ttu-id="0d30a-138">Die Anzeige oder der angezeigte Name des Rollenbereichs Tags.</span><span class="sxs-lookup"><span data-stu-id="0d30a-138">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="0d30a-139">description</span><span class="sxs-lookup"><span data-stu-id="0d30a-139">description</span></span>|<span data-ttu-id="0d30a-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d30a-140">String</span></span>|<span data-ttu-id="0d30a-141">Beschreibung des Rollenbereichs Tags.</span><span class="sxs-lookup"><span data-stu-id="0d30a-141">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="0d30a-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d30a-142">Response</span></span>
<span data-ttu-id="0d30a-143">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [roleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0d30a-143">If successful, this method returns a `200 OK` response code and an updated [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d30a-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0d30a-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d30a-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d30a-145">Request</span></span>
<span data-ttu-id="0d30a-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0d30a-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0d30a-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d30a-147">Response</span></span>
<span data-ttu-id="0d30a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d30a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




