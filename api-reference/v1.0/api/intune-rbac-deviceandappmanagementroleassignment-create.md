---
title: DeviceAndAppManagementRoleAssignment erstellen
description: Erstellen eines neuen deviceAndAppManagementRoleAssignment-Objekts.
author: tfitzmac
ms.openlocfilehash: dc2227837d1652e32353df6aaba96596276ce8c9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305656"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="483d1-103">DeviceAndAppManagementRoleAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="483d1-103">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="483d1-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="483d1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="483d1-105">Erstellen eines neuen [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="483d1-105">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="483d1-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="483d1-106">Prerequisites</span></span>
<span data-ttu-id="483d1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="483d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="483d1-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="483d1-109">Permission type</span></span>|<span data-ttu-id="483d1-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="483d1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="483d1-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="483d1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="483d1-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="483d1-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="483d1-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="483d1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="483d1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="483d1-114">Not supported.</span></span>|
|<span data-ttu-id="483d1-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="483d1-115">Application</span></span>|<span data-ttu-id="483d1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="483d1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="483d1-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="483d1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="483d1-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="483d1-118">Request headers</span></span>
|<span data-ttu-id="483d1-119">Header</span><span class="sxs-lookup"><span data-stu-id="483d1-119">Header</span></span>|<span data-ttu-id="483d1-120">Wert</span><span class="sxs-lookup"><span data-stu-id="483d1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="483d1-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="483d1-121">Authorization</span></span>|<span data-ttu-id="483d1-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="483d1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="483d1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="483d1-123">Accept</span></span>|<span data-ttu-id="483d1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="483d1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="483d1-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="483d1-125">Request body</span></span>
<span data-ttu-id="483d1-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceAndAppManagementRoleAssignment an.</span><span class="sxs-lookup"><span data-stu-id="483d1-126">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="483d1-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceAndAppManagementRoleAssignment erstellen.</span><span class="sxs-lookup"><span data-stu-id="483d1-127">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="483d1-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="483d1-128">Property</span></span>|<span data-ttu-id="483d1-129">Typ</span><span class="sxs-lookup"><span data-stu-id="483d1-129">Type</span></span>|<span data-ttu-id="483d1-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="483d1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="483d1-131">id</span><span class="sxs-lookup"><span data-stu-id="483d1-131">id</span></span>|<span data-ttu-id="483d1-132">String</span><span class="sxs-lookup"><span data-stu-id="483d1-132">String</span></span>|<span data-ttu-id="483d1-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="483d1-133">Key of the entity.</span></span> <span data-ttu-id="483d1-134">Dies ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="483d1-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="483d1-135">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="483d1-135">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="483d1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="483d1-136">displayName</span></span>|<span data-ttu-id="483d1-137">String</span><span class="sxs-lookup"><span data-stu-id="483d1-137">String</span></span>|<span data-ttu-id="483d1-138">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="483d1-138">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="483d1-139">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="483d1-139">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="483d1-140">description</span><span class="sxs-lookup"><span data-stu-id="483d1-140">description</span></span>|<span data-ttu-id="483d1-141">String</span><span class="sxs-lookup"><span data-stu-id="483d1-141">String</span></span>|<span data-ttu-id="483d1-142">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="483d1-142">Description of the Role Assignment.</span></span> <span data-ttu-id="483d1-143">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="483d1-143">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="483d1-144">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="483d1-144">resourceScopes</span></span>|<span data-ttu-id="483d1-145">String collection</span><span class="sxs-lookup"><span data-stu-id="483d1-145">String collection</span></span>|<span data-ttu-id="483d1-146">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="483d1-146">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="483d1-147">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="483d1-147">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="483d1-148">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="483d1-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="483d1-149">Elemente</span><span class="sxs-lookup"><span data-stu-id="483d1-149">members</span></span>|<span data-ttu-id="483d1-150">String collection</span><span class="sxs-lookup"><span data-stu-id="483d1-150">String collection</span></span>|<span data-ttu-id="483d1-151">Die Liste der IDs der Rollenmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="483d1-151">The list of ids of role member security groups.</span></span> <span data-ttu-id="483d1-152">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="483d1-152">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="483d1-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="483d1-153">Response</span></span>
<span data-ttu-id="483d1-154">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="483d1-154">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="483d1-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="483d1-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="483d1-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="483d1-156">Request</span></span>
<span data-ttu-id="483d1-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="483d1-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
Content-type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="483d1-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="483d1-158">Response</span></span>
<span data-ttu-id="483d1-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="483d1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 307

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```



