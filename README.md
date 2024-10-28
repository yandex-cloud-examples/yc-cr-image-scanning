# Автоматическое сканирование Docker-образа при загрузке

В этом руководстве вы создадите [реестр](https://yandex.cloud/ru/docs/container-registry/concepts/registry) [Container Registry](https://yandex.cloud/ru/docs/container-registry/) для хранения Docker-образа и настроите автоматическое сканирование на уязвимости, при загрузке образа в реестр. С помощью триггера [Cloud Functions](https://yandex.cloud/ru/docs/functions/) будут отслеживаться изменения в реестре и при загрузке Docker-образа в реестр, будет вызываться функция для запуска сканирования.

Подготовка инфраструктуры для создания рееестра и настройки автоматические сканирования Docker-образов с помощью Terraform описана в [практическом руководстве](https://yandex.cloud/ru/docs/container-registry/tutorials/image-auto-scan), необходимые для настройки конфигурационные файлы `image-auto-scan.tf` и `image-auto-scan.auto.tfvars` и `function.zip` расположены в этом репозитории.
