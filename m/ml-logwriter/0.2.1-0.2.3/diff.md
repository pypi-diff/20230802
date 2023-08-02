# Comparing `tmp/ml_logwriter-0.2.1.tar.gz` & `tmp/ml_logwriter-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_logwriter-0.2.1.tar", last modified: Wed Aug  2 03:35:46 2023, max compression
+gzip compressed data, was "ml_logwriter-0.2.3.tar", last modified: Wed Aug  2 13:38:53 2023, max compression
```

## Comparing `ml_logwriter-0.2.1.tar` & `ml_logwriter-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 03:35:45.998669 ml_logwriter-0.2.1/
--rw-rw-rw-   0        0        0     1098 2023-07-19 02:50:37.000000 ml_logwriter-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     6365 2023-08-02 03:35:45.997669 ml_logwriter-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     5855 2023-08-02 03:29:44.000000 ml_logwriter-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 03:35:45.993566 ml_logwriter-0.2.1/ml_logwriter/
--rw-rw-rw-   0        0        0        0 2023-07-19 22:28:38.000000 ml_logwriter-0.2.1/ml_logwriter/__init__.py
--rw-rw-rw-   0        0        0     8658 2023-08-02 03:29:44.000000 ml_logwriter-0.2.1/ml_logwriter/loggers.py
-drwxrwxrwx   0        0        0        0 2023-08-02 03:35:45.997669 ml_logwriter-0.2.1/ml_logwriter.egg-info/
--rw-rw-rw-   0        0        0     6365 2023-08-02 03:35:45.000000 ml_logwriter-0.2.1/ml_logwriter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-08-02 03:35:45.000000 ml_logwriter-0.2.1/ml_logwriter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 03:35:45.000000 ml_logwriter-0.2.1/ml_logwriter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-08-02 03:35:45.000000 ml_logwriter-0.2.1/ml_logwriter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 03:35:45.998669 ml_logwriter-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      427 2023-08-02 03:21:17.000000 ml_logwriter-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:38:53.375287 ml_logwriter-0.2.3/
+-rw-rw-rw-   0        0        0     1098 2023-07-19 02:50:37.000000 ml_logwriter-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     6185 2023-08-02 13:38:53.373781 ml_logwriter-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5887 2023-08-02 13:25:37.000000 ml_logwriter-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 13:38:53.360758 ml_logwriter-0.2.3/ml_logwriter/
+-rw-rw-rw-   0        0        0       21 2023-08-02 13:38:47.000000 ml_logwriter-0.2.3/ml_logwriter/__init__.py
+-rw-rw-rw-   0        0        0     8658 2023-08-02 03:29:44.000000 ml_logwriter-0.2.3/ml_logwriter/loggers.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:38:53.371260 ml_logwriter-0.2.3/ml_logwriter.egg-info/
+drwxrwxrwx   0        0        0        0 2023-08-02 13:38:53.373781 ml_logwriter-0.2.3/ml_logwriter.egg-info/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0     6185 2023-08-02 13:35:07.000000 ml_logwriter-0.2.3/ml_logwriter.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rw-rw-rw-   0        0        0      219 2023-08-02 13:35:07.000000 ml_logwriter-0.2.3/ml_logwriter.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 13:35:07.000000 ml_logwriter-0.2.3/ml_logwriter.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-rw-rw-   0        0        0       13 2023-08-02 13:35:07.000000 ml_logwriter-0.2.3/ml_logwriter.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-rw-rw-   0        0        0     6185 2023-08-02 13:38:53.000000 ml_logwriter-0.2.3/ml_logwriter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2023-08-02 13:38:53.000000 ml_logwriter-0.2.3/ml_logwriter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 13:38:53.000000 ml_logwriter-0.2.3/ml_logwriter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-08-02 13:38:53.000000 ml_logwriter-0.2.3/ml_logwriter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 13:38:53.375287 ml_logwriter-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      445 2023-08-02 13:38:29.000000 ml_logwriter-0.2.3/setup.py
```

### Comparing `ml_logwriter-0.2.1/LICENSE` & `ml_logwriter-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_logwriter-0.2.1/PKG-INFO` & `ml_logwriter-0.2.3/ml_logwriter.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
-Name: ml_logwriter
-Version: 0.2.1
+Name: ml-logwriter
+Version: 0.2.2
 Summary: A ML logger package
 Home-page: https://github.com/pedrohrafael/ml-logwriter
 Author: Pedro H Rafael
 Author-email: pedro.rodrigues.rafael@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Machine Learning __LogWriter__
 
 **ML LogWriter:** Biblioteca para Registro de Logs e Armazenamento de Artefatos
 
-## DescriÃ§Ã£o
-O ML LogWriter Ã© uma biblioteca Python de cÃ³digo aberto disponibilizada que visa facilitar o registro de logs de execuÃ§Ã£o de cÃ³digo e o armazenamento de artefatos de modelos em projetos de aprendizado de mÃ¡quina e experimentos de ciÃªncia de dados. 
+## Descrição
+O ML LogWriter é uma biblioteca Python de código aberto disponibilizada que visa facilitar o registro de logs de execução de código e o armazenamento de artefatos de modelos em projetos de aprendizado de máquina e experimentos de ciência de dados. 
 
-Com duas classes principais, `LogWriter` e `LogArtifacts`, essa biblioteca oferece uma soluÃ§Ã£o simples e eficiente para acompanhar o desempenho de modelos e registrar informaÃ§Ãµes essenciais durante o desenvolvimento de projetos.
+Com duas classes principais, `LogWriter` e `LogArtifacts`, essa biblioteca oferece uma solução simples e eficiente para acompanhar o desempenho de modelos e registrar informações essenciais durante o desenvolvimento de projetos.
 
-## MÃ³dulos
+## Módulos
 ### LogWriter:
-A classe LogWriter Ã© responsÃ¡vel por registrar logs de execuÃ§Ã£o em dois locais simultaneamente: em um arquivo de log e no terminal. Suas principais funcionalidades incluem:
+A classe LogWriter é responsável por registrar logs de execução em dois locais simultaneamente: em um arquivo de log e no terminal. Suas principais funcionalidades incluem:
 
-Registro detalhado de eventos: Possibilita registrar informaÃ§Ãµes relevantes em diferentes nÃ­veis de detalhe (por exemplo, INFO, WARNING, ERROR) para auxiliar na depuraÃ§Ã£o e monitoramento da execuÃ§Ã£o do cÃ³digo.
-- **Armazenamento em arquivo:** Registra as informaÃ§Ãµes em um arquivo de log, permitindo revisitar eventos passados e manter um histÃ³rico de execuÃ§Ãµes.
-- **SaÃ­da no terminal:** Exibe informaÃ§Ãµes importantes diretamente no terminal, facilitando o acompanhamento do progresso do cÃ³digo em tempo real.
+Registro detalhado de eventos: Possibilita registrar informações relevantes em diferentes níveis de detalhe (por exemplo, INFO, WARNING, ERROR) para auxiliar na depuração e monitoramento da execução do código.
+- **Armazenamento em arquivo:** Registra as informações em um arquivo de log, permitindo revisitar eventos passados e manter um histórico de execuções.
+- **Saída no terminal:** Exibe informações importantes diretamente no terminal, facilitando o acompanhamento do progresso do código em tempo real.
 
-#### Exemplo de uso do mÃ³dulo `LogWriter`:
+#### Exemplo de uso do módulo `LogWriter`:
 ```python
-# Importando a classe LogWriter do mÃ³dulo
-from log_module import LogWriter
+# Importando a classe LogWriter do módulo
+from ml_logwriter.loggers import LogWriter
 
-# Criando uma instÃ¢ncia da classe LogWriter e definindo o caminho para o arquivo de log
+# Criando uma instância da classe LogWriter e definindo o caminho para o arquivo de log
 log_writer = LogWriter()
 log_path = 'logs/log_file.txt'
 
 # Obtendo o logger para fazer os registros de log
 logger = log_writer.logger(log_path)
 
 # Exemplo de uso do logger para fazer registros de log
@@ -45,75 +45,73 @@
 logger.error("Error message: This is an error log.")
 logger.critical("Critical message: This is a critical log.")
 ```
 
 ### LogArtifacts:
 A classe LogArtifacts foi desenvolvida para armazenar e organizar artefatos essenciais de experimentos e modelos. Suas principais funcionalidades incluem:
 
-- **Armazenamento de modelos e metadados:** Permite salvar modelos treinados juntamente com metadados relevantes, como hiperparÃ¢metros e mÃ©tricas de desempenho.
-- **Gerenciamento de experimentos:** Organiza os resultados de experimentos em uma estrutura de diretÃ³rios clara e consistente, facilitando a localizaÃ§Ã£o e comparaÃ§Ã£o entre diferentes iteraÃ§Ãµes de modelos.
-- **Armazenamento de dados e grÃ¡ficos:** AlÃ©m dos modelos, a classe LogArtifacts Ã© capaz de armazenar outros artefatos, como conjuntos de dados, grÃ¡ficos de desempenho e imagens relevantes para a anÃ¡lise dos resultados.
+- **Armazenamento de modelos e metadados:** Permite salvar modelos treinados juntamente com metadados relevantes, como hiperparâmetros e métricas de desempenho.
+- **Gerenciamento de experimentos:** Organiza os resultados de experimentos em uma estrutura de diretórios clara e consistente, facilitando a localização e comparação entre diferentes iterações de modelos.
+- **Armazenamento de dados e gráficos:** Além dos modelos, a classe LogArtifacts é capaz de armazenar outros artefatos, como conjuntos de dados, gráficos de desempenho e imagens relevantes para a análise dos resultados.
 
-#### Exemplo de Uso do MÃ³dulo `LogArtifacts`:
+#### Exemplo de Uso do Módulo `LogArtifacts`:
 
 ```python
-# Importando a classe LogArtifacts do mÃ³dulo
-from log_module import LogArtifacts
+# Importando a classe LogArtifacts do módulo
+from ml_logwriter.loggers import LogArtifacts
 
-# Criando uma instÃ¢ncia da classe LogArtifacts e definindo o caminho para o diretÃ³rio de artefatos
+# Criando uma instância da classe LogArtifacts e definindo o caminho para o diretório de artefatos (já existente)
 artifacts_path = 'artifacts'
 
-# Criando um novo diretÃ³rio de artefatos (experimento)
+# Criando um novo diretório de artefatos (experimento)
 experiment = LogArtifacts(artifacts_path)
 experiment.create()
 
-# Exemplo de uso da classe LogArtifacts para registrar parÃ¢metros, mÃ©tricas, modelo e dataset
+# Exemplo de uso da classe LogArtifacts para registrar parâmetros, métricas, modelo e dataset
 parameters = {'learning_rate': 0.01, 'batch_size': 32, 'num_epochs': 50}
 metrics = {'accuracy': 0.85, 'precision': 0.78, 'recall': 0.92}
 model = 'Trained Model Object'
 dataset = pd.DataFrame({'feature1': [1, 2, 3], 'feature2': [4, 5, 6]})
 
 experiment.log_parameters(parameters)
 experiment.log_metrics(metrics)
 experiment.log_model(model)
 experiment.log_dataset(dataset, 'example_dataset')
 
-# Criando um grÃ¡fico de desempenho (exemplo com valores aleatÃ³rios)
+# Criando um gráfico de desempenho (exemplo com valores aleatórios)
 x_values = [1, 2, 3, 4, 5]
 y_values = [0.9, 0.85, 0.78, 0.75, 0.72]
 experiment.log_performance_graph(x_values, y_values, title='Model Performance',
                                  x_label='Epoch', y_label='Accuracy', filename='accuracy_graph')
 
-# ApÃ³s executar o cÃ³digo acima, vocÃª verÃ¡ os artefatos salvos no diretÃ³rio 'artifacts' com os resultados do experimento.
+# Após executar o código acima, você verá os artefatos salvos no diretório 'artifacts' com os resultados do experimento.
 ```
 
-## Principais BenefÃ­cios
+## Principais Benefícios
 
 - **Facilidade de Uso:** Com uma interface intuitiva, a biblioteca permite que desenvolvedores e cientistas de dados incorporem facilmente a funcionalidade de registro de logs e armazenamento de artefatos em seus projetos.
-- **OrganizaÃ§Ã£o e Rastreabilidade:** O ML LogWriter facilita a organizaÃ§Ã£o de experimentos e a rastreabilidade de modelos, permitindo que os usuÃ¡rios acessem informaÃ§Ãµes histÃ³ricas e comparem resultados de forma sistemÃ¡tica.
-- **ColaboraÃ§Ã£o Eficiente:** Ao armazenar artefatos e logs em arquivos, a biblioteca possibilita a colaboraÃ§Ã£o entre membros da equipe, uma vez que todos os envolvidos podem compartilhar informaÃ§Ãµes e resultados relevantes.
-- **Melhoria no Processo de Desenvolvimento:** Com o registro detalhado de logs e a capacidade de armazenar artefatos, o ML LogWriter auxilia no processo de depuraÃ§Ã£o, otimizaÃ§Ã£o de modelos e tomada de decisÃµes com base em mÃ©tricas objetivas.
+- **Organização e Rastreabilidade:** O ML LogWriter facilita a organização de experimentos e a rastreabilidade de modelos, permitindo que os usuários acessem informações históricas e comparem resultados de forma sistemática.
+- **Colaboração Eficiente:** Ao armazenar artefatos e logs em arquivos, a biblioteca possibilita a colaboração entre membros da equipe, uma vez que todos os envolvidos podem compartilhar informações e resultados relevantes.
+- **Melhoria no Processo de Desenvolvimento:** Com o registro detalhado de logs e a capacidade de armazenar artefatos, o ML LogWriter auxilia no processo de depuração, otimização de modelos e tomada de decisões com base em métricas objetivas.
 
-## InstalaÃ§Ã£o
+## Instalação
 ```python
 pip install ml-logwriter
 ```
 
 ## Requisitos
-O ML LogWriter requer a instalaÃ§Ã£o das bibliotecas Python necessÃ¡rias para funcionar corretamente.
+O ML LogWriter requer a instalação das bibliotecas Python necessárias para funcionar corretamente.
 ```
 DateTime==5.2
 joblib==1.3.1
 logging==0.4.9.6
 pytz==2023.3
 zope.interface==6.0
 matplotlib==3.7.0
 ```
 Ou instale executando:
 ```python
 pip install -r requirements.txt
 ```
 
-
-
-## ContribuiÃ§Ã£o e LicenÃ§a:
-A biblioteca ML LogWriter Ã© de cÃ³digo aberto e Ã© incentivada a contribuiÃ§Ã£o da comunidade para o seu aprimoramento. Ela estÃ¡ licenciada sob a LicenÃ§a MIT, garantindo liberdade de uso e modificaÃ§Ã£o para qualquer projeto, seja comercial ou nÃ£o.
+## Contribuição e Licença:
+A biblioteca ML LogWriter é de código aberto e é incentivada a contribuição da comunidade para o seu aprimoramento. Ela está licenciada sob a Licença MIT, garantindo liberdade de uso e modificação para qualquer projeto, seja comercial ou não.
```

### Comparing `ml_logwriter-0.2.1/README.md` & `ml_logwriter-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 Registro detalhado de eventos: Possibilita registrar informações relevantes em diferentes níveis de detalhe (por exemplo, INFO, WARNING, ERROR) para auxiliar na depuração e monitoramento da execução do código.
 - **Armazenamento em arquivo:** Registra as informações em um arquivo de log, permitindo revisitar eventos passados e manter um histórico de execuções.
 - **Saída no terminal:** Exibe informações importantes diretamente no terminal, facilitando o acompanhamento do progresso do código em tempo real.
 
 #### Exemplo de uso do módulo `LogWriter`:
 ```python
 # Importando a classe LogWriter do módulo
-from log_module import LogWriter
+from ml_logwriter.loggers import LogWriter
 
 # Criando uma instância da classe LogWriter e definindo o caminho para o arquivo de log
 log_writer = LogWriter()
 log_path = 'logs/log_file.txt'
 
 # Obtendo o logger para fazer os registros de log
 logger = log_writer.logger(log_path)
@@ -42,17 +42,17 @@
 - **Gerenciamento de experimentos:** Organiza os resultados de experimentos em uma estrutura de diretórios clara e consistente, facilitando a localização e comparação entre diferentes iterações de modelos.
 - **Armazenamento de dados e gráficos:** Além dos modelos, a classe LogArtifacts é capaz de armazenar outros artefatos, como conjuntos de dados, gráficos de desempenho e imagens relevantes para a análise dos resultados.
 
 #### Exemplo de Uso do Módulo `LogArtifacts`:
 
 ```python
 # Importando a classe LogArtifacts do módulo
-from log_module import LogArtifacts
+from ml_logwriter.loggers import LogArtifacts
 
-# Criando uma instância da classe LogArtifacts e definindo o caminho para o diretório de artefatos
+# Criando uma instância da classe LogArtifacts e definindo o caminho para o diretório de artefatos (já existente)
 artifacts_path = 'artifacts'
 
 # Criando um novo diretório de artefatos (experimento)
 experiment = LogArtifacts(artifacts_path)
 experiment.create()
 
 # Exemplo de uso da classe LogArtifacts para registrar parâmetros, métricas, modelo e dataset
@@ -98,11 +98,9 @@
 matplotlib==3.7.0
 ```
 Ou instale executando:
 ```python
 pip install -r requirements.txt
 ```
 
-
-
 ## Contribuição e Licença:
 A biblioteca ML LogWriter é de código aberto e é incentivada a contribuição da comunidade para o seu aprimoramento. Ela está licenciada sob a Licença MIT, garantindo liberdade de uso e modificação para qualquer projeto, seja comercial ou não.
```

### Comparing `ml_logwriter-0.2.1/ml_logwriter/loggers.py` & `ml_logwriter-0.2.3/ml_logwriter/loggers.py`

 * *Files identical despite different names*

### Comparing `ml_logwriter-0.2.1/ml_logwriter.egg-info/PKG-INFO` & `ml_logwriter-0.2.3/ml_logwriter.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: ml-logwriter
-Version: 0.2.1
+Version: 0.2.3
 Summary: A ML logger package
 Home-page: https://github.com/pedrohrafael/ml-logwriter
 Author: Pedro H Rafael
 Author-email: pedro.rodrigues.rafael@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Machine Learning __LogWriter__
 
 **ML LogWriter:** Biblioteca para Registro de Logs e Armazenamento de Artefatos
 
-## DescriÃ§Ã£o
-O ML LogWriter Ã© uma biblioteca Python de cÃ³digo aberto disponibilizada que visa facilitar o registro de logs de execuÃ§Ã£o de cÃ³digo e o armazenamento de artefatos de modelos em projetos de aprendizado de mÃ¡quina e experimentos de ciÃªncia de dados. 
+## Descrição
+O ML LogWriter é uma biblioteca Python de código aberto disponibilizada que visa facilitar o registro de logs de execução de código e o armazenamento de artefatos de modelos em projetos de aprendizado de máquina e experimentos de ciência de dados. 
 
-Com duas classes principais, `LogWriter` e `LogArtifacts`, essa biblioteca oferece uma soluÃ§Ã£o simples e eficiente para acompanhar o desempenho de modelos e registrar informaÃ§Ãµes essenciais durante o desenvolvimento de projetos.
+Com duas classes principais, `LogWriter` e `LogArtifacts`, essa biblioteca oferece uma solução simples e eficiente para acompanhar o desempenho de modelos e registrar informações essenciais durante o desenvolvimento de projetos.
 
-## MÃ³dulos
+## Módulos
 ### LogWriter:
-A classe LogWriter Ã© responsÃ¡vel por registrar logs de execuÃ§Ã£o em dois locais simultaneamente: em um arquivo de log e no terminal. Suas principais funcionalidades incluem:
+A classe LogWriter é responsável por registrar logs de execução em dois locais simultaneamente: em um arquivo de log e no terminal. Suas principais funcionalidades incluem:
 
-Registro detalhado de eventos: Possibilita registrar informaÃ§Ãµes relevantes em diferentes nÃ­veis de detalhe (por exemplo, INFO, WARNING, ERROR) para auxiliar na depuraÃ§Ã£o e monitoramento da execuÃ§Ã£o do cÃ³digo.
-- **Armazenamento em arquivo:** Registra as informaÃ§Ãµes em um arquivo de log, permitindo revisitar eventos passados e manter um histÃ³rico de execuÃ§Ãµes.
-- **SaÃ­da no terminal:** Exibe informaÃ§Ãµes importantes diretamente no terminal, facilitando o acompanhamento do progresso do cÃ³digo em tempo real.
+Registro detalhado de eventos: Possibilita registrar informações relevantes em diferentes níveis de detalhe (por exemplo, INFO, WARNING, ERROR) para auxiliar na depuração e monitoramento da execução do código.
+- **Armazenamento em arquivo:** Registra as informações em um arquivo de log, permitindo revisitar eventos passados e manter um histórico de execuções.
+- **Saída no terminal:** Exibe informações importantes diretamente no terminal, facilitando o acompanhamento do progresso do código em tempo real.
 
-#### Exemplo de uso do mÃ³dulo `LogWriter`:
+#### Exemplo de uso do módulo `LogWriter`:
 ```python
-# Importando a classe LogWriter do mÃ³dulo
-from log_module import LogWriter
+# Importando a classe LogWriter do módulo
+from ml_logwriter.loggers import LogWriter
 
-# Criando uma instÃ¢ncia da classe LogWriter e definindo o caminho para o arquivo de log
+# Criando uma instância da classe LogWriter e definindo o caminho para o arquivo de log
 log_writer = LogWriter()
 log_path = 'logs/log_file.txt'
 
 # Obtendo o logger para fazer os registros de log
 logger = log_writer.logger(log_path)
 
 # Exemplo de uso do logger para fazer registros de log
@@ -45,75 +45,73 @@
 logger.error("Error message: This is an error log.")
 logger.critical("Critical message: This is a critical log.")
 ```
 
 ### LogArtifacts:
 A classe LogArtifacts foi desenvolvida para armazenar e organizar artefatos essenciais de experimentos e modelos. Suas principais funcionalidades incluem:
 
-- **Armazenamento de modelos e metadados:** Permite salvar modelos treinados juntamente com metadados relevantes, como hiperparÃ¢metros e mÃ©tricas de desempenho.
-- **Gerenciamento de experimentos:** Organiza os resultados de experimentos em uma estrutura de diretÃ³rios clara e consistente, facilitando a localizaÃ§Ã£o e comparaÃ§Ã£o entre diferentes iteraÃ§Ãµes de modelos.
-- **Armazenamento de dados e grÃ¡ficos:** AlÃ©m dos modelos, a classe LogArtifacts Ã© capaz de armazenar outros artefatos, como conjuntos de dados, grÃ¡ficos de desempenho e imagens relevantes para a anÃ¡lise dos resultados.
+- **Armazenamento de modelos e metadados:** Permite salvar modelos treinados juntamente com metadados relevantes, como hiperparâmetros e métricas de desempenho.
+- **Gerenciamento de experimentos:** Organiza os resultados de experimentos em uma estrutura de diretórios clara e consistente, facilitando a localização e comparação entre diferentes iterações de modelos.
+- **Armazenamento de dados e gráficos:** Além dos modelos, a classe LogArtifacts é capaz de armazenar outros artefatos, como conjuntos de dados, gráficos de desempenho e imagens relevantes para a análise dos resultados.
 
-#### Exemplo de Uso do MÃ³dulo `LogArtifacts`:
+#### Exemplo de Uso do Módulo `LogArtifacts`:
 
 ```python
-# Importando a classe LogArtifacts do mÃ³dulo
-from log_module import LogArtifacts
+# Importando a classe LogArtifacts do módulo
+from ml_logwriter.loggers import LogArtifacts
 
-# Criando uma instÃ¢ncia da classe LogArtifacts e definindo o caminho para o diretÃ³rio de artefatos
+# Criando uma instância da classe LogArtifacts e definindo o caminho para o diretório de artefatos (já existente)
 artifacts_path = 'artifacts'
 
-# Criando um novo diretÃ³rio de artefatos (experimento)
+# Criando um novo diretório de artefatos (experimento)
 experiment = LogArtifacts(artifacts_path)
 experiment.create()
 
-# Exemplo de uso da classe LogArtifacts para registrar parÃ¢metros, mÃ©tricas, modelo e dataset
+# Exemplo de uso da classe LogArtifacts para registrar parâmetros, métricas, modelo e dataset
 parameters = {'learning_rate': 0.01, 'batch_size': 32, 'num_epochs': 50}
 metrics = {'accuracy': 0.85, 'precision': 0.78, 'recall': 0.92}
 model = 'Trained Model Object'
 dataset = pd.DataFrame({'feature1': [1, 2, 3], 'feature2': [4, 5, 6]})
 
 experiment.log_parameters(parameters)
 experiment.log_metrics(metrics)
 experiment.log_model(model)
 experiment.log_dataset(dataset, 'example_dataset')
 
-# Criando um grÃ¡fico de desempenho (exemplo com valores aleatÃ³rios)
+# Criando um gráfico de desempenho (exemplo com valores aleatórios)
 x_values = [1, 2, 3, 4, 5]
 y_values = [0.9, 0.85, 0.78, 0.75, 0.72]
 experiment.log_performance_graph(x_values, y_values, title='Model Performance',
                                  x_label='Epoch', y_label='Accuracy', filename='accuracy_graph')
 
-# ApÃ³s executar o cÃ³digo acima, vocÃª verÃ¡ os artefatos salvos no diretÃ³rio 'artifacts' com os resultados do experimento.
+# Após executar o código acima, você verá os artefatos salvos no diretório 'artifacts' com os resultados do experimento.
 ```
 
-## Principais BenefÃ­cios
+## Principais Benefícios
 
 - **Facilidade de Uso:** Com uma interface intuitiva, a biblioteca permite que desenvolvedores e cientistas de dados incorporem facilmente a funcionalidade de registro de logs e armazenamento de artefatos em seus projetos.
-- **OrganizaÃ§Ã£o e Rastreabilidade:** O ML LogWriter facilita a organizaÃ§Ã£o de experimentos e a rastreabilidade de modelos, permitindo que os usuÃ¡rios acessem informaÃ§Ãµes histÃ³ricas e comparem resultados de forma sistemÃ¡tica.
-- **ColaboraÃ§Ã£o Eficiente:** Ao armazenar artefatos e logs em arquivos, a biblioteca possibilita a colaboraÃ§Ã£o entre membros da equipe, uma vez que todos os envolvidos podem compartilhar informaÃ§Ãµes e resultados relevantes.
-- **Melhoria no Processo de Desenvolvimento:** Com o registro detalhado de logs e a capacidade de armazenar artefatos, o ML LogWriter auxilia no processo de depuraÃ§Ã£o, otimizaÃ§Ã£o de modelos e tomada de decisÃµes com base em mÃ©tricas objetivas.
+- **Organização e Rastreabilidade:** O ML LogWriter facilita a organização de experimentos e a rastreabilidade de modelos, permitindo que os usuários acessem informações históricas e comparem resultados de forma sistemática.
+- **Colaboração Eficiente:** Ao armazenar artefatos e logs em arquivos, a biblioteca possibilita a colaboração entre membros da equipe, uma vez que todos os envolvidos podem compartilhar informações e resultados relevantes.
+- **Melhoria no Processo de Desenvolvimento:** Com o registro detalhado de logs e a capacidade de armazenar artefatos, o ML LogWriter auxilia no processo de depuração, otimização de modelos e tomada de decisões com base em métricas objetivas.
 
-## InstalaÃ§Ã£o
+## Instalação
 ```python
 pip install ml-logwriter
 ```
 
 ## Requisitos
-O ML LogWriter requer a instalaÃ§Ã£o das bibliotecas Python necessÃ¡rias para funcionar corretamente.
+O ML LogWriter requer a instalação das bibliotecas Python necessárias para funcionar corretamente.
 ```
 DateTime==5.2
 joblib==1.3.1
 logging==0.4.9.6
 pytz==2023.3
 zope.interface==6.0
 matplotlib==3.7.0
 ```
 Ou instale executando:
 ```python
 pip install -r requirements.txt
 ```
 
-
-
-## ContribuiÃ§Ã£o e LicenÃ§a:
-A biblioteca ML LogWriter Ã© de cÃ³digo aberto e Ã© incentivada a contribuiÃ§Ã£o da comunidade para o seu aprimoramento. Ela estÃ¡ licenciada sob a LicenÃ§a MIT, garantindo liberdade de uso e modificaÃ§Ã£o para qualquer projeto, seja comercial ou nÃ£o.
+## Contribuição e Licença:
+A biblioteca ML LogWriter é de código aberto e é incentivada a contribuição da comunidade para o seu aprimoramento. Ela está licenciada sob a Licença MIT, garantindo liberdade de uso e modificação para qualquer projeto, seja comercial ou não.
```

