---
title: DeviceAndAppManagementRoleAssignment erstellen
description: Erstellen eines neuen deviceAndAppManagementRoleAssignment-Objekts.
ms.openlocfilehash: ec8c641ca9d3d4d4f42cfe71f44bcb6f216be273
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066209"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="eaaa8-103">DeviceAndAppManagementRoleAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="eaaa8-103">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="eaaa8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eaaa8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eaaa8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eaaa8-107">Erstellen eines neuen [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-107">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eaaa8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eaaa8-108">Prerequisites</span></span>
<span data-ttu-id="eaaa8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaaa8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaaa8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eaaa8-111">Permission type</span></span>|<span data-ttu-id="eaaa8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eaaa8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eaaa8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eaaa8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eaaa8-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaaa8-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="eaaa8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eaaa8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eaaa8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eaaa8-116">Not supported.</span></span>|
|<span data-ttu-id="eaaa8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eaaa8-117">Application</span></span>|<span data-ttu-id="eaaa8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eaaa8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eaaa8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eaaa8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="eaaa8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eaaa8-120">Request headers</span></span>
|<span data-ttu-id="eaaa8-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="eaaa8-121">Header</span></span>|<span data-ttu-id="eaaa8-122">Wert</span><span class="sxs-lookup"><span data-stu-id="eaaa8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eaaa8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eaaa8-123">Authorization</span></span>|<span data-ttu-id="eaaa8-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eaaa8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eaaa8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eaaa8-125">Accept</span></span>|<span data-ttu-id="eaaa8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eaaa8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eaaa8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eaaa8-127">Request body</span></span>
<span data-ttu-id="eaaa8-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceAndAppManagementRoleAssignment an.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-128">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="eaaa8-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceAndAppManagementRoleAssignment erstellen.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-129">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="eaaa8-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eaaa8-130">Property</span></span>|<span data-ttu-id="eaaa8-131">Typ</span><span class="sxs-lookup"><span data-stu-id="eaaa8-131">Type</span></span>|<span data-ttu-id="eaaa8-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eaaa8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaaa8-133">id</span><span class="sxs-lookup"><span data-stu-id="eaaa8-133">id</span></span>|<span data-ttu-id="eaaa8-134">String</span><span class="sxs-lookup"><span data-stu-id="eaaa8-134">String</span></span>|<span data-ttu-id="eaaa8-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="eaaa8-135">Key of the entity.</span></span> <span data-ttu-id="eaaa8-136">Dies ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="eaaa8-137">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="eaaa8-137">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="eaaa8-138">displayName</span><span class="sxs-lookup"><span data-stu-id="eaaa8-138">displayName</span></span>|<span data-ttu-id="eaaa8-139">String</span><span class="sxs-lookup"><span data-stu-id="eaaa8-139">String</span></span>|<span data-ttu-id="eaaa8-140">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-140">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="eaaa8-141">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="eaaa8-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="eaaa8-142">description</span><span class="sxs-lookup"><span data-stu-id="eaaa8-142">description</span></span>|<span data-ttu-id="eaaa8-143">String</span><span class="sxs-lookup"><span data-stu-id="eaaa8-143">String</span></span>|<span data-ttu-id="eaaa8-144">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-144">Description of the Role Assignment.</span></span> <span data-ttu-id="eaaa8-145">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="eaaa8-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="eaaa8-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="eaaa8-146">scopeMembers</span></span>|<span data-ttu-id="eaaa8-147">String collection</span><span class="sxs-lookup"><span data-stu-id="eaaa8-147">String collection</span></span>|<span data-ttu-id="eaaa8-148">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="eaaa8-149">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-149">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="eaaa8-150">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="eaaa8-150">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="eaaa8-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="eaaa8-151">scopeType</span></span>|[<span data-ttu-id="eaaa8-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="eaaa8-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="eaaa8-153">Gibt den Typ des Bereichs für eine Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="eaaa8-154">Standardtyp 'ResourceScope' ermöglicht die Zuweisung von ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="eaaa8-155">Für 'AllDevices', 'AllLicensedUsers' und 'AllDevicesAndLicensedUsers' sollte die ResourceScopes-Eigenschaft leer bleiben.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="eaaa8-156">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="eaaa8-156">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="eaaa8-157">Mögliche Werte: sind `resourceScope`, `allDevices`, `allLicensedUsers` und `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-157">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="eaaa8-158">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="eaaa8-158">resourceScopes</span></span>|<span data-ttu-id="eaaa8-159">String collection</span><span class="sxs-lookup"><span data-stu-id="eaaa8-159">String collection</span></span>|<span data-ttu-id="eaaa8-160">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-160">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="eaaa8-161">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-161">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="eaaa8-162">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="eaaa8-162">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="eaaa8-163">Elemente</span><span class="sxs-lookup"><span data-stu-id="eaaa8-163">members</span></span>|<span data-ttu-id="eaaa8-164">String collection</span><span class="sxs-lookup"><span data-stu-id="eaaa8-164">String collection</span></span>|<span data-ttu-id="eaaa8-165">Die Liste der IDs der Rollenmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-165">The list of ids of role member security groups.</span></span> <span data-ttu-id="eaaa8-166">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-166">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="eaaa8-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="eaaa8-167">Response</span></span>
<span data-ttu-id="eaaa8-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-168">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaaa8-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eaaa8-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="eaaa8-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eaaa8-170">Request</span></span>
<span data-ttu-id="eaaa8-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleAssignments
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="eaaa8-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="eaaa8-172">Response</span></span>
<span data-ttu-id="eaaa8-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eaaa8-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 391

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```





