# Создание графика с помощью текстового запроса

Для создания графика с помощью текстового запроса выполните следующее:

1. На главной странице сервиса [!KEYREF monitoring-full-name] нажмите **Создать график**.
1. В разделе **Запросы** нажмите значок ![image](../../_assets/ellipsis.svg) и выберите пункт **Редактировать как текст**.
1. Укажите через запятую обязательные метки с необходимыми значениями:

    ```
    project="your_project_name", cluster="your_cluster_name", service="service_name"
    ```
1. Укажите дополнительные метки, чтобы вывести метрики на график.
    
    > [!IMPORTANT]
    >
    > На один график можно добавить не более 50 метрик.

1. Нажмите значок ![image](../../_assets/checkmark.png). Метрика отобразится на графике.
1. Нажмите **Завершить**. В открывшемся окне введите имя графика и выберите папку, в которой он будет сохранен.
1. Нажмите **Сохранить**. График сохранится в указанной папке.

## Пример запроса

Запрос метрики `disk_read_bytes` виртуальной машины сервиса [!KEYREF compute-full-name]:
```
project="project_id", cluster="cluster_id", service="compute", resource_type="vm", resource_id="resource_id", name="disk_read_bytes"
```