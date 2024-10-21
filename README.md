# Ingestao-Incremental-Streaming
O Auto Loader é um recurso do Apache Spark que facilita a ingestão incremental de dados em tempo real. Ele permite a leitura automática de novos arquivos em um diretório (sistema de arquivos, podendo conter diversos formatos, nesse caso são arquivos .json), aplicando um esquema definido e gerenciando checkpoints para garantir a consistência dos dados. Esses dados (arquivos .json nesse projeto) são então carregados em uma tabela em um banco de dados.

Com o Auto Loader, os dados são ingeridos de forma atômica, garantindo que não haja perda de informações em caso de falhas no processo de carregamento. Essa abordagem é especialmente útil para cenários de big data, onde grandes volumes de dados são gerados constantemente, proporcionando uma solução eficiente e resiliente para a ingestão de dados.

### Checkpoints gerados:

![checkpoints_autoloader](https://github.com/user-attachments/assets/86dcdd98-70be-4114-be2b-79d946377e82)

Este projeto foi desenvolvido para fins demonstrativos usando o Azure Databricks, fazendo o uso do Hive metastore, com uma ingestão incremental de streaming de arquivos [.json]. Você pode container o código e usá-lo como microserviço, bem como armazenar em diferentes destinos, e processar dados de diferentes fontes.
