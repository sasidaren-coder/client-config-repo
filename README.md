# client-config-repo
Confluent Cloud Client Config Repo


# For Local testing only:


cd /Users/sasidarendinakaran/Documents/<Client>/Internals/Automation/<Client>_automation_v2/local_tf_executions/terragrunt_impls/client-config-repo/azure/dev/topics


export CLOUD_PROVIDER=azure
export ENV=dev
export CONFLUENT_API_KEY=<CC API Key>
export CONFLUENT_API_SECRET=<CC API Secret>
export KAFKA_API_KEY=<Kafka API Key>
export KAFKA_API_SECRET=<Kafka API Secret>
export KAFKA_CLUSTER_ID=<Kafka Cluster ID>
export KAFKA_REST_ENDPOINT=https://<DNS>:443
export AZURE_RESOURCE_GROUP_NAME=<Azure RG>
export AZURE_STORAGE_ACCOUNT_NAME=<Azure Storage Account>
export AZURE_STORAGE_CONTAINER_NAME=<Azure Container name>

terragrunt init --source /Users/sasidarendinakaran/Documents/<Client>/Internals/Automation/<Client>_automation_v2/local_tf_executions/terragrunt_impls/iac-modules/modules//kafka-topics

terragrunt plan --source /Users/sasidarendinakaran/Documents/<Client>/Internals/Automation/<Client>_automation_v2/local_tf_executions/terragrunt_impls/iac-modules/modules//kafka-topics

terragrunt apply --source /Users/sasidarendinakaran/Documents/<Client>/Internals/Automation/<Client>_automation_v2/local_tf_executions/terragrunt_impls/iac-modules/modules//kafka-topics