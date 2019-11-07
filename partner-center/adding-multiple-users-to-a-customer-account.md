---
title: Создание нескольких пользователей для учетной записи клиента | Центр партнеров
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Вы можете добавить несколько пользователей к учетной записи клиента одновременно, загрузив файл данных в формате CSV в Центр партнеров.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
ms.author: evansma
keywords: массовая отправка, добавление нескольких пользователей в учетную запись клиента, добавление пользователей клиента, массовая отправка пользователей клиента, учетная запись клиента, пользователи клиента, пользователи
ms.localizationpriority: medium
ms.openlocfilehash: 4062c36d9f5d394d9d25eb67265784d2a5b301cf
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653244"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="ea556-104">Добавление нескольких пользователей к учетной записи клиента</span><span class="sxs-lookup"><span data-stu-id="ea556-104">Add multiple users to a customer account</span></span>

<span data-ttu-id="ea556-105">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="ea556-105">**Applies to**</span></span>

-  <span data-ttu-id="ea556-106">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="ea556-106">Partner Center</span></span>

<span data-ttu-id="ea556-107">Можно одновременно добавить нескольких пользователей в учетную запись клиента, открыв файл данных в формате файла с разделителями-запятыми (CSV) в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="ea556-107">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="ea556-108">Вы можете скачать образец файла данных из центра партнеров, а затем изменить его для использования или создать новый файл данных, используя модель данных, определенную ниже.</span><span class="sxs-lookup"><span data-stu-id="ea556-108">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="ea556-109">Требования к файлам данных</span><span class="sxs-lookup"><span data-stu-id="ea556-109">Data file requirements</span></span>


<span data-ttu-id="ea556-110">Чтобы добавить нескольких пользователей в учетную запись клиента с помощью процесса групповой отправки, необходимо выполнить следующие требования.</span><span class="sxs-lookup"><span data-stu-id="ea556-110">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

-   <span data-ttu-id="ea556-111">у вас должны быть разрешения глобального администратора для учетной записи клиента;</span><span class="sxs-lookup"><span data-stu-id="ea556-111">You must have global administrator permissions to the customer account;</span></span>
-   <span data-ttu-id="ea556-112">у каждого пользователя должен быть уникальный электронный адрес в почтовом домене пользователя;</span><span class="sxs-lookup"><span data-stu-id="ea556-112">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
-   <span data-ttu-id="ea556-113">одновременно можно передавать до 100 записей.</span><span class="sxs-lookup"><span data-stu-id="ea556-113">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="ea556-114">Если вам необходимо добавить более 100 пользователей, создайте и загрузите дополнительные файлы данных;</span><span class="sxs-lookup"><span data-stu-id="ea556-114">If you need to add more than 100 users, create and upload additional data files.</span></span>
-   <span data-ttu-id="ea556-115">все пользователи должны быть в одном географическом **регионе**;</span><span class="sxs-lookup"><span data-stu-id="ea556-115">All users must be in the same geographic **Location**.</span></span>
-   <span data-ttu-id="ea556-116">вводите только данные, описанные ниже.</span><span class="sxs-lookup"><span data-stu-id="ea556-116">Enter only the data described below.</span></span> <span data-ttu-id="ea556-117">Лишние данные приведут к ошибке отправки.</span><span class="sxs-lookup"><span data-stu-id="ea556-117">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="ea556-118">Введите следующие данные в файле данных:</span><span class="sxs-lookup"><span data-stu-id="ea556-118">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="ea556-119">**Имя столбца**</span><span class="sxs-lookup"><span data-stu-id="ea556-119">**Column name**</span></span> | <span data-ttu-id="ea556-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ea556-120">**Description**</span></span>                                                              | <span data-ttu-id="ea556-121">**Чего**</span><span class="sxs-lookup"><span data-stu-id="ea556-121">**Limitation**</span></span>                             |
| <span data-ttu-id="ea556-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ea556-122">First name</span></span>      | <span data-ttu-id="ea556-123">Имя пользователя (необязательное поле)</span><span class="sxs-lookup"><span data-stu-id="ea556-123">User's first name (optional field)</span></span>                                           | <span data-ttu-id="ea556-124">Ограничение в 50 символов</span><span class="sxs-lookup"><span data-stu-id="ea556-124">50-character limit</span></span>                         |
| <span data-ttu-id="ea556-125">Фамилия</span><span class="sxs-lookup"><span data-stu-id="ea556-125">Last name</span></span>       | <span data-ttu-id="ea556-126">Фамилия пользователя (обязательное поле)</span><span class="sxs-lookup"><span data-stu-id="ea556-126">User's last name (optional field)</span></span>                                            | <span data-ttu-id="ea556-127">Ограничение в 50 символов</span><span class="sxs-lookup"><span data-stu-id="ea556-127">50-character limit</span></span>                         |
| <span data-ttu-id="ea556-128">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="ea556-128">Display name</span></span>    | <span data-ttu-id="ea556-129">Имя, отображаемое в центре партнеров (обязательное поле)</span><span class="sxs-lookup"><span data-stu-id="ea556-129">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="ea556-130">Ограничение в 50 символов</span><span class="sxs-lookup"><span data-stu-id="ea556-130">50-character limit</span></span>                         |
| <span data-ttu-id="ea556-131">Электронная почта</span><span class="sxs-lookup"><span data-stu-id="ea556-131">Email</span></span>           | <span data-ttu-id="ea556-132">Рабочий адрес электронной почты пользователя в клиентской компании (обязательное поле)</span><span class="sxs-lookup"><span data-stu-id="ea556-132">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="ea556-133">У каждого пользователя должен быть уникальный электронный адрес</span><span class="sxs-lookup"><span data-stu-id="ea556-133">Each user must have a unique email address</span></span> |
| <span data-ttu-id="ea556-134">Обновление состояния</span><span class="sxs-lookup"><span data-stu-id="ea556-134">Status update</span></span>   | <span data-ttu-id="ea556-135">Используется для указания того, была ли новая запись пользователя успешно создана</span><span class="sxs-lookup"><span data-stu-id="ea556-135">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="ea556-136">\*\*оставить пустым\*\*</span><span class="sxs-lookup"><span data-stu-id="ea556-136">\*\*Leave empty\*\*</span></span>                        |

 

### <a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="ea556-137">Создание нескольких учетных записей пользователей</span><span class="sxs-lookup"><span data-stu-id="ea556-137">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>
1.  <span data-ttu-id="ea556-138">Создайте файл данных с разделителями-запятыми (CSV) с данными, описанными выше.</span><span class="sxs-lookup"><span data-stu-id="ea556-138">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="ea556-139">Сохраните файл, чтобы выбрать его позднее.</span><span class="sxs-lookup"><span data-stu-id="ea556-139">Save the file so you can browse to it in a later step.</span></span>
2.  <span data-ttu-id="ea556-140">В меню **Центр партнеров** выберите **Клиенты**, а затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="ea556-140">From the **Partner Center** menu, select **Customers**, then choose a customer from the list.</span></span>
3.  <span data-ttu-id="ea556-141">Выберите **Отправить пользователей**.</span><span class="sxs-lookup"><span data-stu-id="ea556-141">Select **Upload users**.</span></span>
4.  <span data-ttu-id="ea556-142">В разделе **Передача данных пользователя** нажмите кнопку **Обзор**.</span><span class="sxs-lookup"><span data-stu-id="ea556-142">Under **Upload user info**, select **Browse**.</span></span>
5.  <span data-ttu-id="ea556-143">В средство выбора файлов выберите ваш файл данных, а затем нажмите **Открыть**.</span><span class="sxs-lookup"><span data-stu-id="ea556-143">In the file selector, select your data file and then select **Open**.</span></span>
6.  <span data-ttu-id="ea556-144">Выберите **Проверить**.</span><span class="sxs-lookup"><span data-stu-id="ea556-144">Select **Validate**.</span></span>

    <span data-ttu-id="ea556-145">**Примечание** .  большинство ошибок создания учетной записи вызваны проблемами с файлами данных, в том числе отсутствующими сведениями, неправильно сформированными или повторяющимися адресами электронной почты или слишком большим числом записей в файле.</span><span class="sxs-lookup"><span data-stu-id="ea556-145">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

7.  <span data-ttu-id="ea556-146">После того как центр партнеров проверит файл, выберите географическое **Расположение** для новых пользователей.</span><span class="sxs-lookup"><span data-stu-id="ea556-146">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
8.  <span data-ttu-id="ea556-147">Выберите **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="ea556-147">Select **Save**.</span></span>
9.  <span data-ttu-id="ea556-148">Скачайте данные о временных паролях для пользователей.</span><span class="sxs-lookup"><span data-stu-id="ea556-148">Download the temporary password information for the users.</span></span>

<span data-ttu-id="ea556-149">**ВАЖНО.** Обязательно скачайте файла с временными паролями сейчас, так как потом это будет невозможно.</span><span class="sxs-lookup"><span data-stu-id="ea556-149">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="ea556-150">Новым пользователям необходимо выполнить вход в новую учетную запись, используя временный пароль.</span><span class="sxs-lookup"><span data-stu-id="ea556-150">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="ea556-151">Новым пользователям автоматически назначаются разрешения **Может использовать лицензии и службы**.</span><span class="sxs-lookup"><span data-stu-id="ea556-151">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



