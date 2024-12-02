1. RDS (Amazon Relational Database Service)
Métricas de desempenho:
CPUUtilization
DatabaseConnections
FreeStorageSpace
ReadIOPS / WriteIOPS
ReadThroughput / WriteThroughput
ReplicaLag
DiskQueueDepth
NetworkReceiveThroughput / NetworkTransmitThroughput
Métricas de Latência:
Latency (para leituras e escritas)
2. EKS (Amazon Elastic Kubernetes Service)
Cluster Health:
pod.count
pod.running
pod.pending
pod.failed
node.active / node.unavailable
Utilização de Recursos:
MemoryUtilization
CPUUtilization
DiskUtilization
NetworkReceiveBytes / NetworkTransmitBytes
Métricas do Kubernetes via Prometheus:
Container CPU Usage (container_cpu_usage_seconds_total)
Container Memory Usage (container_memory_working_set_bytes)
Container Restarts (kube_pod_container_status_restarts_total)
3. EC2 (Amazon Elastic Compute Cloud)
Desempenho da Instância:
CPUUtilization
DiskReadOps / DiskWriteOps
NetworkIn / NetworkOut
StatusCheckFailed / StatusCheckFailed_Instance / StatusCheckFailed_System
EBS Metrics:
VolumeReadBytes / VolumeWriteBytes
VolumeReadOps / VolumeWriteOps
BurstBalance
4. Elastic Load Balancer (ELB/ALB/NLB)
Desempenho:
RequestCount
Latency
HealthyHostCount / UnHealthyHostCount
Erros:
HTTPCode_ELB_4XX_Count / HTTPCode_ELB_5XX_Count
HTTPCode_Backend_4XX_Count / HTTPCode_Backend_5XX_Count
5. Lambda (AWS Lambda Functions)
Execução:
Invocations
Errors
Throttles
Duration
IteratorAge (para funções processando streams)
Conexões:
ConcurrentExecutions
UnreservedConcurrentExecutions
6. Kafka (Amazon MSK ou Custom)
Tópicos e Produção:
BytesInPerSec / BytesOutPerSec
MessagesInPerSec
PartitionCount
Lag:
ConsumerLagSum
MaxLag
Brokers:
CPUUtilization
DiskUtilization
NetworkIn / NetworkOut
7. S3 (Amazon Simple Storage Service)
Armazenamento:
BucketSizeBytes
NumberOfObjects
Solicitações:
AllRequests
GetRequests / PutRequests / DeleteRequests
4xxErrors / 5xxErrors
8. ECS (Amazon Elastic Container Service)
Tasks:
MemoryUtilization
CPUUtilization
RunningTaskCount / PendingTaskCount
Network:
NetworkRxBytes / NetworkTxBytes
StorageReadBytes / StorageWriteBytes
9. CloudFront
Performance:
Requests
BytesDownloaded / BytesUploaded
CacheHitRate / CacheMissRate
Erros:
4xxErrorRate
5xxErrorRate
10. DynamoDB
Capacidade:
ReadCapacityUnits
WriteCapacityUnits
Erros:
ThrottledRequests
UserErrors
Latência:
SuccessfulRequestLatency
11. VPC (Amazon Virtual Private Cloud)
Tráfego:
BytesIn / BytesOut
PacketsIn / PacketsOut
Conexões:
ActiveFlowCount
FlowLogs (via logs para análise de segurança)
12. SNS (Amazon Simple Notification Service)
Mensagens:
NumberOfMessagesPublished
NumberOfNotificationsDelivered
PublishSize
Erros:
NumberOfNotificationsFailed
DeliveryRetries
13. SQS (Amazon Simple Queue Service)
Mensagens:
NumberOfMessagesSent
NumberOfMessagesReceived
NumberOfMessagesDeleted
ApproximateNumberOfMessagesDelayed
Erros:
SentMessageSize
ApproximateAgeOfOldestMessage
14. API Gateway
Tráfego:
Count
IntegrationLatency
Latency
Erros:
4XXError
5XXError
15. Outros Serviços Comuns
Elasticache: CPUUtilization, SwapUsage, FreeableMemory, Evictions.
Kinesis: IncomingRecords, IncomingBytes, WriteProvisionedThroughputExceeded.
Athena: QueryExecutionTime, QueryScannedBytes.
