---
title: Создание нескольких пользователей для учетной записи клиента | Центр партнеров
description: Вы можете добавить несколько пользователей к учетной записи клиента одновременно, загрузив файл данных в формате CSV в Центр партнеров.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
keywords: массовая отправка, добавление нескольких пользователей в учетную запись клиента, добавление пользователей клиента, массовая отправка пользователей клиента, учетная запись клиента, пользователи клиента, пользователи
ms.localizationpriority: medium
ms.openlocfilehash: 123c2c7b80398a860aa894449052502d41409c85
ms.sourcegitcommit: 123a7f53d633c27eb5f982926d856de47afb1042
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2018
ms.locfileid: "4488820"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="562c8-104">Добавление нескольких пользователей к учетной записи клиента</span><span class="sxs-lookup"><span data-stu-id="562c8-104">Add multiple users to a customer account</span></span>

**<span data-ttu-id="562c8-105">Относится к:</span><span class="sxs-lookup"><span data-stu-id="562c8-105">Applies to</span></span>**

-  <span data-ttu-id="562c8-106">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="562c8-106">Partner Center</span></span>

<span data-ttu-id="562c8-107">Можно добавить несколько пользователей учетной записи клиента одновременно, загрузив файл данных с разделителями-запятыми (.csv) в центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="562c8-107">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="562c8-108">Можно скачать пример файла данных в центре партнеров и изменить его для себя или можете создать новый файл данных с помощью модели данных, описанной ниже.</span><span class="sxs-lookup"><span data-stu-id="562c8-108">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="562c8-109">Требования к файлу данных</span><span class="sxs-lookup"><span data-stu-id="562c8-109">Data file requirements</span></span>


<span data-ttu-id="562c8-110">Чтобы добавить несколько пользователей к учетной записи клиента с помощью пакетной загрузки, вам необходимо соблюдать следующие требования:</span><span class="sxs-lookup"><span data-stu-id="562c8-110">To add multiple users to a customer’s account using the bulk upload process, you’ll need to meet the following requirements:</span></span>

-   <span data-ttu-id="562c8-111">у вас должны быть разрешения глобального администратора для учетной записи клиента;</span><span class="sxs-lookup"><span data-stu-id="562c8-111">You must have global administrator permissions to the customer account;</span></span>
-   <span data-ttu-id="562c8-112">у каждого пользователя должен быть уникальный электронный адрес в почтовом домене пользователя;</span><span class="sxs-lookup"><span data-stu-id="562c8-112">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
-   <span data-ttu-id="562c8-113">одновременно можно передавать до 100 записей.</span><span class="sxs-lookup"><span data-stu-id="562c8-113">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="562c8-114">Если вам необходимо добавить более 100 пользователей, создайте и загрузите дополнительные файлы данных;</span><span class="sxs-lookup"><span data-stu-id="562c8-114">If you need to add more than 100 users, create and upload additional data files.</span></span>
-   <span data-ttu-id="562c8-115">все пользователи должны быть в одном географическом **регионе**;</span><span class="sxs-lookup"><span data-stu-id="562c8-115">All users must be in the same geographic **Location**.</span></span>
-   <span data-ttu-id="562c8-116">вводите только данные, описанные ниже.</span><span class="sxs-lookup"><span data-stu-id="562c8-116">Enter only the data described below.</span></span> <span data-ttu-id="562c8-117">Лишние данные приведут к ошибке отправки.</span><span class="sxs-lookup"><span data-stu-id="562c8-117">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="562c8-118">Введите следующие данные в файле данных:</span><span class="sxs-lookup"><span data-stu-id="562c8-118">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **<span data-ttu-id="562c8-119">Имя столбца</span><span class="sxs-lookup"><span data-stu-id="562c8-119">Column name</span></span>** | **<span data-ttu-id="562c8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="562c8-120">Description</span></span>**                                                              | **<span data-ttu-id="562c8-121">Ограничение</span><span class="sxs-lookup"><span data-stu-id="562c8-121">Limitation</span></span>**                             |
| <span data-ttu-id="562c8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="562c8-122">First name</span></span>      | <span data-ttu-id="562c8-123">Имя пользователя (обязательное поле)</span><span class="sxs-lookup"><span data-stu-id="562c8-123">User’s first name (optional field)</span></span>                                           | <span data-ttu-id="562c8-124">Ограничение в 50 символов</span><span class="sxs-lookup"><span data-stu-id="562c8-124">50-character limit</span></span>                         |
| <span data-ttu-id="562c8-125">Фамилия</span><span class="sxs-lookup"><span data-stu-id="562c8-125">Last name</span></span>       | <span data-ttu-id="562c8-126">Фамилия пользователя (обязательное поле)</span><span class="sxs-lookup"><span data-stu-id="562c8-126">User's last name (optional field)</span></span>                                            | <span data-ttu-id="562c8-127">Ограничение в 50 символов</span><span class="sxs-lookup"><span data-stu-id="562c8-127">50-character limit</span></span>                         |
| <span data-ttu-id="562c8-128">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="562c8-128">Display name</span></span>    | <span data-ttu-id="562c8-129">Имя, отображаемое в центре партнеров (обязательное поле)</span><span class="sxs-lookup"><span data-stu-id="562c8-129">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="562c8-130">Ограничение в 50 символов</span><span class="sxs-lookup"><span data-stu-id="562c8-130">50-character limit</span></span>                         |
| <span data-ttu-id="562c8-131">Электронный адрес</span><span class="sxs-lookup"><span data-stu-id="562c8-131">Email</span></span>           | <span data-ttu-id="562c8-132">Рабочий электронный адрес компании клиента (обязательное поле)</span><span class="sxs-lookup"><span data-stu-id="562c8-132">User’s business email address at customer company (required field)</span></span>           | <span data-ttu-id="562c8-133">У каждого пользователя должен быть уникальный электронный адрес</span><span class="sxs-lookup"><span data-stu-id="562c8-133">Each user must have a unique email address</span></span> |
| <span data-ttu-id="562c8-134">Обновление состояния</span><span class="sxs-lookup"><span data-stu-id="562c8-134">Status update</span></span>   | <span data-ttu-id="562c8-135">Используется для указания того, была ли новая запись пользователя успешно создана</span><span class="sxs-lookup"><span data-stu-id="562c8-135">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="562c8-136">\*\*Оставить пустым\*\*</span><span class="sxs-lookup"><span data-stu-id="562c8-136">\*\*Leave empty\*\*</span></span>                        |

 

### <a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="562c8-137">Создание нескольких учетных записей пользователей</span><span class="sxs-lookup"><span data-stu-id="562c8-137">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>
1.  <span data-ttu-id="562c8-138">Создайте файл данных с разделителями-запятыми (CSV) с данными, описанными выше.</span><span class="sxs-lookup"><span data-stu-id="562c8-138">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="562c8-139">Сохраните файл, чтобы выбрать его позднее.</span><span class="sxs-lookup"><span data-stu-id="562c8-139">Save the file so you can browse to it in a later step.</span></span>
2.  <span data-ttu-id="562c8-140">В меню **Центра партнеров** выберите **пользователей**, а затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="562c8-140">From the **Partner Center** menu, select **Customers**, then choose a customer from the list.</span></span>
3.  <span data-ttu-id="562c8-141">Выберите **Отправить пользователей**.</span><span class="sxs-lookup"><span data-stu-id="562c8-141">Select **Upload users**.</span></span>
4.  <span data-ttu-id="562c8-142">В разделе **Передача данных пользователя** нажмите кнопку **Обзор**.</span><span class="sxs-lookup"><span data-stu-id="562c8-142">Under **Upload user info**, select **Browse**.</span></span>
5.  <span data-ttu-id="562c8-143">В средство выбора файлов выберите ваш файл данных, а затем нажмите **Открыть**.</span><span class="sxs-lookup"><span data-stu-id="562c8-143">In the file selector, select your data file and then select **Open**.</span></span>
6.  <span data-ttu-id="562c8-144">Выберите **Проверить**.</span><span class="sxs-lookup"><span data-stu-id="562c8-144">Select **Validate**.</span></span>

    <span data-ttu-id="562c8-145">**Примечание**. Большинство ошибок при создании учетной записи вызваны проблемами с файлом данных, такими как отсутствие информации, некорректные или повторяющиеся электронные адреса, слишком много записей в файле и т. д.</span><span class="sxs-lookup"><span data-stu-id="562c8-145">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

7.  <span data-ttu-id="562c8-146">После проверки файла в центре партнеров выберите географическое **расположение** для новых пользователей.</span><span class="sxs-lookup"><span data-stu-id="562c8-146">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
8.  <span data-ttu-id="562c8-147">Выберите **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="562c8-147">Select **Save**.</span></span>
9.  <span data-ttu-id="562c8-148">Скачайте данные о временных паролях для пользователей.</span><span class="sxs-lookup"><span data-stu-id="562c8-148">Download the temporary password information for the users.</span></span>

<span data-ttu-id="562c8-149">**ВАЖНО.** Обязательно скачайте файла с временными паролями сейчас, так как потом это будет невозможно.</span><span class="sxs-lookup"><span data-stu-id="562c8-149">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="562c8-150">Новым пользователям необходимо выполнить вход в новую учетную запись, используя временный пароль.</span><span class="sxs-lookup"><span data-stu-id="562c8-150">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="562c8-151">Новые пользователи автоматически назначаются разрешения **можно использовать лицензии и службы** .</span><span class="sxs-lookup"><span data-stu-id="562c8-151">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



