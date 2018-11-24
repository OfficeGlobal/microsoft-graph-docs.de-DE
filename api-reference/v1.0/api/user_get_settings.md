# <a name="get-settings"></a><span data-ttu-id="43f42-101">Abrufen von Einstellungen</span><span class="sxs-lookup"><span data-stu-id="43f42-101">Get settings</span></span>

<span data-ttu-id="43f42-102">Lesen Sie Benutzer- und [Settings](../resources/user_settings.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="43f42-102">Read the user and organization [settings](../resources/user_settings.md) object.</span></span>
<span data-ttu-id="43f42-103">Weitere Informationen zum Aktualisieren der Eigenschaften des [Settings](../resources/user_settings.md) -Objekts finden Sie unter [Aktualisieren von benutzereinstellungen](user_update_settings.md).</span><span class="sxs-lookup"><span data-stu-id="43f42-103">To learn how to update the properties of the [settings](../resources/user_settings.md) object, see [update user settings](user_update_settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="43f42-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="43f42-104">Permissions</span></span>

<span data-ttu-id="43f42-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="43f42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="43f42-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="43f42-107">Permission type</span></span>      | <span data-ttu-id="43f42-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="43f42-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43f42-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="43f42-109">Delegated (work or school account)</span></span> | <span data-ttu-id="43f42-110">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43f42-110">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="43f42-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="43f42-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43f42-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43f42-112">Not supported.</span></span>    |
|<span data-ttu-id="43f42-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="43f42-113">Application</span></span> | <span data-ttu-id="43f42-114">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43f42-114">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="43f42-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="43f42-115">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="43f42-116">Fordern Sie mit einer 'Benutzer-Id"oder"UserPrincipalName"ist nur verfügbar, durch den Benutzer oder von einem Benutzer mit den Berechtigungen User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="43f42-116">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="43f42-117">Weitere Informationen finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="43f42-117">To learn more, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="43f42-118">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="43f42-118">Request body</span></span>

<span data-ttu-id="43f42-119">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="43f42-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43f42-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="43f42-120">Response</span></span>

<span data-ttu-id="43f42-121">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [Einstellungen](../resources/user_settings.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="43f42-121">If successful, this method returns a `200 OK` response code and [user settings](../resources/user_settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43f42-122">Beispiel</span><span class="sxs-lookup"><span data-stu-id="43f42-122">Example</span></span>

##### <a name="request"></a><span data-ttu-id="43f42-123">Anforderung</span><span class="sxs-lookup"><span data-stu-id="43f42-123">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a><span data-ttu-id="43f42-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="43f42-124">Response</span></span>

<span data-ttu-id="43f42-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="43f42-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```

