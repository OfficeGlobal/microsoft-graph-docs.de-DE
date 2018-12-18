---
title: RoleScopeTag aktualisieren
description: Aktualisieren Sie die Eigenschaften eines RoleScopeTag-Objekts.
author: tfitzmac
ms.openlocfilehash: 3e1cdc0997e0c2f7ebb8d70c730785e40b4143d4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306944"
---
# <a name="update-rolescopetag"></a><span data-ttu-id="1d168-103">RoleScopeTag aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1d168-103">Update roleScopeTag</span></span>

> <span data-ttu-id="1d168-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1d168-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d168-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1d168-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d168-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1d168-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d168-107">Aktualisieren Sie die Eigenschaften eines [RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="1d168-107">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1d168-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1d168-108">Prerequisites</span></span>
<span data-ttu-id="1d168-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d168-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d168-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1d168-111">Permission type</span></span>|<span data-ttu-id="1d168-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1d168-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d168-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1d168-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d168-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d168-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="1d168-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1d168-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d168-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1d168-116">Not supported.</span></span>|
|<span data-ttu-id="1d168-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1d168-117">Application</span></span>|<span data-ttu-id="1d168-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1d168-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d168-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d168-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleScopeTags/{roleScopeTagId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="request-headers"></a><span data-ttu-id="1d168-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1d168-120">Request headers</span></span>
|<span data-ttu-id="1d168-121">Header</span><span class="sxs-lookup"><span data-stu-id="1d168-121">Header</span></span>|<span data-ttu-id="1d168-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1d168-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d168-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1d168-123">Authorization</span></span>|<span data-ttu-id="1d168-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1d168-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d168-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1d168-125">Accept</span></span>|<span data-ttu-id="1d168-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d168-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d168-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1d168-127">Request body</span></span>
<span data-ttu-id="1d168-128">Geben Sie im Textkörper Anforderung für das Objekt [RoleScopeTag](../resources/intune-rbac-rolescopetag.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="1d168-128">In the request body, supply a JSON representation for the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

<span data-ttu-id="1d168-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [RoleScopeTag](../resources/intune-rbac-rolescopetag.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="1d168-129">The following table shows the properties that are required when you create the [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>

|<span data-ttu-id="1d168-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1d168-130">Property</span></span>|<span data-ttu-id="1d168-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1d168-131">Type</span></span>|<span data-ttu-id="1d168-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d168-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d168-133">id</span><span class="sxs-lookup"><span data-stu-id="1d168-133">id</span></span>|<span data-ttu-id="1d168-134">String</span><span class="sxs-lookup"><span data-stu-id="1d168-134">String</span></span>|<span data-ttu-id="1d168-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1d168-135">Key of the entity.</span></span> <span data-ttu-id="1d168-136">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="1d168-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="1d168-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1d168-137">displayName</span></span>|<span data-ttu-id="1d168-138">String</span><span class="sxs-lookup"><span data-stu-id="1d168-138">String</span></span>|<span data-ttu-id="1d168-139">Das Display oder den Anzeigenamen des Tags Bereich Rolle.</span><span class="sxs-lookup"><span data-stu-id="1d168-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="1d168-140">description</span><span class="sxs-lookup"><span data-stu-id="1d168-140">description</span></span>|<span data-ttu-id="1d168-141">String</span><span class="sxs-lookup"><span data-stu-id="1d168-141">String</span></span>|<span data-ttu-id="1d168-142">Beschreibung des Tags Bereich Rolle.</span><span class="sxs-lookup"><span data-stu-id="1d168-142">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="1d168-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d168-143">Response</span></span>
<span data-ttu-id="1d168-144">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1d168-144">If successful, this method returns a `200 OK` response code and an updated [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d168-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1d168-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="1d168-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d168-146">Request</span></span>
<span data-ttu-id="1d168-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1d168-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="1d168-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d168-148">Response</span></span>
<span data-ttu-id="1d168-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1d168-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





