# docker simple development

## 執行後將開啟以下服務
- seq
- minio
- redis
- rabbitmq
- mongodb
- postgres
- pgadmin

## 需求
- 已安裝 docker & docker-compose
- 還有port不能佔用
    - seq：5341、5342
    - minio：9000、9001
    - redis：6379
    - rabbitmq：15672、5672
    - mongodb：27017
    - postgres：5432
    - pgadmin：5050

## 執行與關閉
啟動：powershell執行./run-docker-compose.ps1  
關閉：powershell執行./stop-docker-compose.ps1  
刪除：powershell執行./down.ps1


## 資料夾說明
data資料夾存放container資料



## 說明
| 服務     | Port  |   類型  | 帳號            | 密碼     |
|----------|-------|:-------:|-----------------|----------|
| seq      | 5342  |    UI   |                 |          |
|          | 5341  | Service |                 |          |
| minio    | 9000  | Service |                 |          |
|          | 9001  |    UI   | root            | 1q2w3E** |
| redis    | 6379  | Service |                 |          |
| mongodb  | 27017 | Service |                 |          |
| postgres | 5432  | Service | postgres        | 1q2w3E*  |
| pgadmin  | 5050  |    UI   | dev@example.com | 1q2w3E*  |
| rabbitmq |15672  |    UI   | admin           | 1q2w3E*  |
|          | 5672  | Service |                 |          |



