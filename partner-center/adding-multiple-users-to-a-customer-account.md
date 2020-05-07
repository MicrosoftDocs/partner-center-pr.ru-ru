---
title: Создание нескольких пользователей для учетной записи клиента | Центр партнеров
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как одновременно добавить нескольких пользователей в учетную запись клиента, передав файл данных в формате файла с разделителями-запятыми (CSV) в центр партнеров.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: массовая отправка, добавление нескольких пользователей в учетную запись клиента, добавление пользователей клиента, массовая отправка пользователей клиента, учетная запись клиента, пользователи клиента, пользователи
ms.localizationpriority: medium
ms.openlocfilehash: 36130f268c9d33217ef3473136ec511f374fb583
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2020
ms.locfileid: "82798632"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="d8594-104">Добавление нескольких пользователей к учетной записи клиента</span><span class="sxs-lookup"><span data-stu-id="d8594-104">Add multiple users to a customer account</span></span>

<span data-ttu-id="d8594-105">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="d8594-105">**Applies to**</span></span>

- <span data-ttu-id="d8594-106">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="d8594-106">Partner Center</span></span>

<span data-ttu-id="d8594-107">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="d8594-107">**Appropriate roles**</span></span>

- <span data-ttu-id="d8594-108">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="d8594-108">Global admin</span></span>

<span data-ttu-id="d8594-109">Можно одновременно добавить нескольких пользователей в учетную запись клиента, открыв файл данных в формате файла с разделителями-запятыми (CSV) в центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="d8594-109">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="d8594-110">Вы можете скачать образец файла данных из центра партнеров, а затем изменить его для использования или создать новый файл данных, используя модель данных, определенную ниже.</span><span class="sxs-lookup"><span data-stu-id="d8594-110">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="d8594-111">Требования к файлу данных</span><span class="sxs-lookup"><span data-stu-id="d8594-111">Data file requirements</span></span>

<span data-ttu-id="d8594-112">Чтобы добавить нескольких пользователей в учетную запись клиента с помощью процесса групповой отправки, необходимо выполнить следующие требования.</span><span class="sxs-lookup"><span data-stu-id="d8594-112">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="d8594-113">у вас должны быть разрешения глобального администратора для учетной записи клиента;</span><span class="sxs-lookup"><span data-stu-id="d8594-113">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="d8594-114">у каждого пользователя должен быть уникальный электронный адрес в почтовом домене пользователя;</span><span class="sxs-lookup"><span data-stu-id="d8594-114">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="d8594-115">одновременно можно передавать до 100 записей.</span><span class="sxs-lookup"><span data-stu-id="d8594-115">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="d8594-116">Если вам необходимо добавить более 100 пользователей, создайте и загрузите дополнительные файлы данных;</span><span class="sxs-lookup"><span data-stu-id="d8594-116">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="d8594-117">все пользователи должны быть в одном географическом **регионе**;</span><span class="sxs-lookup"><span data-stu-id="d8594-117">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="d8594-118">вводите только данные, описанные ниже.</span><span class="sxs-lookup"><span data-stu-id="d8594-118">Enter only the data described below.</span></span> <span data-ttu-id="d8594-119">Лишние данные приведут к ошибке отправки.</span><span class="sxs-lookup"><span data-stu-id="d8594-119">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="d8594-120">Введите следующие данные в файле данных:</span><span class="sxs-lookup"><span data-stu-id="d8594-120">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="d8594-121">**Имя столбца**</span><span class="sxs-lookup"><span data-stu-id="d8594-121">**Column name**</span></span> | <span data-ttu-id="d8594-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d8594-122">**Description**</span></span>                                                              | <span data-ttu-id="d8594-123">**Чего**</span><span class="sxs-lookup"><span data-stu-id="d8594-123">**Limitation**</span></span>                             |
| <span data-ttu-id="d8594-124">Имя</span><span class="sxs-lookup"><span data-stu-id="d8594-124">First name</span></span>      | <span data-ttu-id="d8594-125">Имя пользователя (необязательное поле)</span><span class="sxs-lookup"><span data-stu-id="d8594-125">User's first name (optional field)</span></span>                                           | <span data-ttu-id="d8594-126">Не более 50 знаков</span><span class="sxs-lookup"><span data-stu-id="d8594-126">50-character limit</span></span>                         |
| <span data-ttu-id="d8594-127">Фамилия</span><span class="sxs-lookup"><span data-stu-id="d8594-127">Last name</span></span>       | <span data-ttu-id="d8594-128">Фамилия пользователя (обязательное поле)</span><span class="sxs-lookup"><span data-stu-id="d8594-128">User's last name (optional field)</span></span>                                            | <span data-ttu-id="d8594-129">Не более 50 знаков</span><span class="sxs-lookup"><span data-stu-id="d8594-129">50-character limit</span></span>                         |
| <span data-ttu-id="d8594-130">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="d8594-130">Display name</span></span>    | <span data-ttu-id="d8594-131">Имя, отображаемое в центре партнеров (обязательное поле)</span><span class="sxs-lookup"><span data-stu-id="d8594-131">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="d8594-132">Не более 50 знаков</span><span class="sxs-lookup"><span data-stu-id="d8594-132">50-character limit</span></span>                         |
| <span data-ttu-id="d8594-133">Электронная почта</span><span class="sxs-lookup"><span data-stu-id="d8594-133">Email</span></span>           | <span data-ttu-id="d8594-134">Рабочий адрес электронной почты пользователя в клиентской компании (обязательное поле)</span><span class="sxs-lookup"><span data-stu-id="d8594-134">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="d8594-135">Каждый пользователь должен иметь уникальный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d8594-135">Each user must have a unique email address</span></span> |
| <span data-ttu-id="d8594-136">Обновление состояния</span><span class="sxs-lookup"><span data-stu-id="d8594-136">Status update</span></span>   | <span data-ttu-id="d8594-137">Используется для указания того, была ли новая запись пользователя успешно создана</span><span class="sxs-lookup"><span data-stu-id="d8594-137">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="d8594-138">\*\*Оставить пустым\*\*</span><span class="sxs-lookup"><span data-stu-id="d8594-138">\*\*Leave empty\*\*</span></span>                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="d8594-139">Создание нескольких учетных записей пользователей</span><span class="sxs-lookup"><span data-stu-id="d8594-139">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>

1. <span data-ttu-id="d8594-140">Создайте файл данных с разделителями-запятыми (CSV) с данными, описанными выше.</span><span class="sxs-lookup"><span data-stu-id="d8594-140">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="d8594-141">Сохраните файл, чтобы выбрать его позднее.</span><span class="sxs-lookup"><span data-stu-id="d8594-141">Save the file so you can browse to it in a later step.</span></span>

2. <span data-ttu-id="d8594-142">Войдите на [панель мониторинга](https://partner.microsoft.com/dashboard) Центра партнеров.</span><span class="sxs-lookup"><span data-stu-id="d8594-142">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="d8594-143">В меню Центра партнеров выберите **Клиенты**, а затем выберите клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="d8594-143">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="d8594-144">Выберите вкладку **Пользователи и лицензии** клиента, а затем щелкните **отправить пользователей**.</span><span class="sxs-lookup"><span data-stu-id="d8594-144">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="d8594-145">В разделе **Передача данных пользователя** нажмите кнопку **Обзор**.</span><span class="sxs-lookup"><span data-stu-id="d8594-145">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="d8594-146">В средство выбора файлов выберите ваш файл данных, а затем нажмите **Открыть**.</span><span class="sxs-lookup"><span data-stu-id="d8594-146">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="d8594-147">Выберите **Проверить**.</span><span class="sxs-lookup"><span data-stu-id="d8594-147">Select **Validate**.</span></span>

    <span data-ttu-id="d8594-148">**Примечание**  . Большинство ошибок создания учетной записи вызвано проблемами с файлами данных, в том числе отсутствующими сведениями, неправильно сформированными или повторяющимися адресами электронной почты или слишком большим числом записей в файле.</span><span class="sxs-lookup"><span data-stu-id="d8594-148">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="d8594-149">После того как центр партнеров проверит файл, выберите географическое **Расположение** для новых пользователей.</span><span class="sxs-lookup"><span data-stu-id="d8594-149">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="d8594-150">Щелкните **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="d8594-150">Select **Save**.</span></span>
10. <span data-ttu-id="d8594-151">Скачайте временный пароль нового пользователя.</span><span class="sxs-lookup"><span data-stu-id="d8594-151">Download the temporary password information for the users.</span></span>

<span data-ttu-id="d8594-152">**ВАЖНО.** Обязательно скачайте файла с временными паролями сейчас, так как потом это будет невозможно.</span><span class="sxs-lookup"><span data-stu-id="d8594-152">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="d8594-153">Новым пользователям необходимо выполнить вход в новую учетную запись, используя временный пароль.</span><span class="sxs-lookup"><span data-stu-id="d8594-153">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="d8594-154">Новым пользователям автоматически назначаются разрешения **Может использовать лицензии и службы**.</span><span class="sxs-lookup"><span data-stu-id="d8594-154">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



