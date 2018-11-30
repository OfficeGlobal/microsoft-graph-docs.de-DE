---
title: roleDefinition erstellen
description: Erstellt neue Objekte des Typs roleDefinition.
ms.openlocfilehash: 6772b065e4d4d73615540667470829b31a2de804
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066182"
---
# <a name="create-roledefinition"></a><span data-ttu-id="cf799-103">roleDefinition erstellen</span><span class="sxs-lookup"><span data-stu-id="cf799-103">Create roleDefinition</span></span>

> <span data-ttu-id="cf799-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cf799-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf799-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cf799-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf799-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cf799-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf799-107">Erstellt neue Objekte des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="cf799-107">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf799-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cf799-108">Prerequisites</span></span>
<span data-ttu-id="cf799-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf799-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf799-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cf799-111">Permission type</span></span>|<span data-ttu-id="cf799-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cf799-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf799-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cf799-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf799-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf799-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="cf799-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cf799-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf799-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf799-116">Not supported.</span></span>|
|<span data-ttu-id="cf799-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cf799-117">Application</span></span>|<span data-ttu-id="cf799-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf799-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf799-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf799-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="cf799-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cf799-120">Request headers</span></span>
|<span data-ttu-id="cf799-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cf799-121">Header</span></span>|<span data-ttu-id="cf799-122">Wert</span><span class="sxs-lookup"><span data-stu-id="cf799-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf799-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf799-123">Authorization</span></span>|<span data-ttu-id="cf799-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cf799-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf799-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf799-125">Accept</span></span>|<span data-ttu-id="cf799-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf799-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf799-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cf799-127">Request body</span></span>
<span data-ttu-id="cf799-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs roleDefinition an.</span><span class="sxs-lookup"><span data-stu-id="cf799-128">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="cf799-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der roleDefinition erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="cf799-129">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="cf799-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cf799-130">Property</span></span>|<span data-ttu-id="cf799-131">Typ</span><span class="sxs-lookup"><span data-stu-id="cf799-131">Type</span></span>|<span data-ttu-id="cf799-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf799-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf799-133">id</span><span class="sxs-lookup"><span data-stu-id="cf799-133">id</span></span>|<span data-ttu-id="cf799-134">String</span><span class="sxs-lookup"><span data-stu-id="cf799-134">String</span></span>|<span data-ttu-id="cf799-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="cf799-135">Key of the entity.</span></span> <span data-ttu-id="cf799-136">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="cf799-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="cf799-137">displayName</span><span class="sxs-lookup"><span data-stu-id="cf799-137">displayName</span></span>|<span data-ttu-id="cf799-138">String</span><span class="sxs-lookup"><span data-stu-id="cf799-138">String</span></span>|<span data-ttu-id="cf799-139">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="cf799-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="cf799-140">description</span><span class="sxs-lookup"><span data-stu-id="cf799-140">description</span></span>|<span data-ttu-id="cf799-141">String</span><span class="sxs-lookup"><span data-stu-id="cf799-141">String</span></span>|<span data-ttu-id="cf799-142">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="cf799-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="cf799-143">permissions</span><span class="sxs-lookup"><span data-stu-id="cf799-143">permissions</span></span>|<span data-ttu-id="cf799-144">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="cf799-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="cf799-145">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="cf799-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="cf799-146">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="cf799-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="cf799-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="cf799-147">rolePermissions</span></span>|<span data-ttu-id="cf799-148">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="cf799-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="cf799-149">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="cf799-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="cf799-150">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="cf799-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="cf799-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cf799-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="cf799-152">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="cf799-152">Boolean</span></span>|<span data-ttu-id="cf799-153">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="cf799-153">Type of Role.</span></span> <span data-ttu-id="cf799-154">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="cf799-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="cf799-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="cf799-155">isBuiltIn</span></span>|<span data-ttu-id="cf799-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="cf799-156">Boolean</span></span>|<span data-ttu-id="cf799-157">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="cf799-157">Type of Role.</span></span> <span data-ttu-id="cf799-158">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="cf799-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="cf799-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf799-159">Response</span></span>
<span data-ttu-id="cf799-160">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [roleDefinition](../resources/intune-rbac-roledefinition.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf799-160">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf799-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cf799-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf799-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf799-162">Request</span></span>
<span data-ttu-id="cf799-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cf799-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
Content-type: application/json
Content-length: 1145

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "displayName": "Display Name value",
  "description": "Description value",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="cf799-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf799-164">Response</span></span>
<span data-ttu-id="cf799-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf799-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1194

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
  "displayName": "Display Name value",
  "description": "Description value",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true
}
```





