---
title: Erstellen von roleScopeTag
description: Erstellen eines neuen RoleScopeTag-Objekts.
author: tfitzmac
ms.openlocfilehash: 2aaede673afa4346a1defbc9449a4e08d9d1c614
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315148"
---
# <a name="create-rolescopetag"></a><span data-ttu-id="ba299-103">Erstellen von roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="ba299-103">Create roleScopeTag</span></span>

> <span data-ttu-id="ba299-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ba299-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba299-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ba299-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ba299-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ba299-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ba299-107">Erstellen eines neuen [RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ba299-107">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ba299-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ba299-108">Prerequisites</span></span>
<span data-ttu-id="ba299-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba299-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba299-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ba299-111">Permission type</span></span>|<span data-ttu-id="ba299-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ba299-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba299-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ba299-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba299-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba299-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="ba299-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ba299-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba299-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ba299-116">Not supported.</span></span>|
|<span data-ttu-id="ba299-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ba299-117">Application</span></span>|<span data-ttu-id="ba299-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ba299-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba299-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ba299-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="ba299-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ba299-120">Request headers</span></span>
|<span data-ttu-id="ba299-121">Header</span><span class="sxs-lookup"><span data-stu-id="ba299-121">Header</span></span>|<span data-ttu-id="ba299-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ba299-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba299-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ba299-123">Authorization</span></span>|<span data-ttu-id="ba299-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ba299-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba299-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ba299-125">Accept</span></span>|<span data-ttu-id="ba299-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ba299-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba299-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ba299-127">Request body</span></span>
<span data-ttu-id="ba299-128">Geben Sie im Textkörper Anforderung für das Objekt RoleScopeTag eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="ba299-128">In the request body, supply a JSON representation for the roleScopeTag object.</span></span>

<span data-ttu-id="ba299-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die RoleScopeTag erstellen.</span><span class="sxs-lookup"><span data-stu-id="ba299-129">The following table shows the properties that are required when you create the roleScopeTag.</span></span>

|<span data-ttu-id="ba299-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ba299-130">Property</span></span>|<span data-ttu-id="ba299-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ba299-131">Type</span></span>|<span data-ttu-id="ba299-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ba299-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba299-133">id</span><span class="sxs-lookup"><span data-stu-id="ba299-133">id</span></span>|<span data-ttu-id="ba299-134">String</span><span class="sxs-lookup"><span data-stu-id="ba299-134">String</span></span>|<span data-ttu-id="ba299-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ba299-135">Key of the entity.</span></span> <span data-ttu-id="ba299-136">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="ba299-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="ba299-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ba299-137">displayName</span></span>|<span data-ttu-id="ba299-138">String</span><span class="sxs-lookup"><span data-stu-id="ba299-138">String</span></span>|<span data-ttu-id="ba299-139">Das Display oder den Anzeigenamen des Tags Bereich Rolle.</span><span class="sxs-lookup"><span data-stu-id="ba299-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="ba299-140">description</span><span class="sxs-lookup"><span data-stu-id="ba299-140">description</span></span>|<span data-ttu-id="ba299-141">String</span><span class="sxs-lookup"><span data-stu-id="ba299-141">String</span></span>|<span data-ttu-id="ba299-142">Beschreibung des Tags Bereich Rolle.</span><span class="sxs-lookup"><span data-stu-id="ba299-142">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="ba299-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="ba299-143">Response</span></span>
<span data-ttu-id="ba299-144">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ba299-144">If successful, this method returns a `201 Created` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba299-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ba299-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="ba299-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ba299-146">Request</span></span>
<span data-ttu-id="ba299-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ba299-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags
Content-type: application/json
Content-length: 133

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="ba299-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="ba299-148">Response</span></span>
<span data-ttu-id="ba299-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ba299-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 182

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
  "displayName": "Display Name value",
  "description": "Description value"
}
```





