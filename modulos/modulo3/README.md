# Módulo 3: Processamento e Análise dos Dados

**Carga Horária:** 6 horas  
**Tipo:** Prático (Laboratório)

## Objetivos de Aprendizagem

Ao final deste módulo, o participante será capaz de:

- Compreender os princípios da fotogrametria digital aplicada a drones
- Processar imagens aéreas em softwares especializados
- Gerar produtos cartográficos de qualidade (ortofotos, MDS, MDT, modelos 3D)
- Realizar análises comparativas entre projeto e execução
- Calcular volumes, áreas e distâncias a partir dos dados processados

## Conteúdo

### 3.1. Introdução à Fotogrametria Digital com Drones

A **fotogrametria** é a ciência e tecnologia de obter informações confiáveis sobre objetos físicos e o ambiente através do registro, medição e interpretação de imagens fotográficas. Com o advento dos drones, a fotogrametria tornou-se mais acessível e eficiente, permitindo a captura de dados aéreos de alta resolução a custos reduzidos.

#### Princípios Básicos

A fotogrametria com drones baseia-se na captura de múltiplas imagens sobrepostas de uma mesma área sob diferentes ângulos. Através de algoritmos de **Structure from Motion (SfM)** e **Multi-View Stereo (MVS)**, o software identifica pontos comuns entre as imagens e reconstrói a geometria tridimensional da cena.

**Etapas do processo fotogramétrico:**

1. **Aquisição de imagens:** Voo com drone capturando fotos com sobreposição adequada
2. **Alinhamento de fotos:** Identificação de pontos homólogos entre imagens
3. **Geração de nuvem de pontos esparsa:** Reconstrução inicial da geometria
4. **Geração de nuvem de pontos densa:** Densificação com milhões de pontos 3D
5. **Geração de malha 3D:** Criação de superfície triangular
6. **Texturização:** Aplicação das cores das fotos na malha
7. **Geração de produtos:** Ortofoto, MDS, MDT

### 3.2. Softwares de Processamento

#### Agisoft Metashape

O **Agisoft Metashape** é um dos softwares mais utilizados para processamento fotogramétrico de imagens de drones. Oferece alta precisão e flexibilidade, sendo amplamente adotado em projetos profissionais de engenharia e mapeamento.

**Características principais:**
- Interface intuitiva e fluxo de trabalho bem definido
- Suporte a diversos formatos de imagem e dados de georreferenciamento
- Processamento em alta qualidade com controle de parâmetros
- Exportação de produtos em múltiplos formatos
- Integração com sistemas de coordenadas e pontos de controle

**Requisitos de hardware:**
- Processador multi-core (recomendado: 8 ou mais núcleos)
- Memória RAM: mínimo 16 GB (recomendado: 32 GB ou mais)
- Placa de vídeo dedicada com suporte a CUDA ou OpenCL
- Espaço em disco: variável conforme o projeto (pode ultrapassar 100 GB)

#### Pix4Dmapper

O **Pix4Dmapper** é uma solução completa para mapeamento com drones, oferecendo processamento rápido e produtos de alta qualidade. É especialmente popular em aplicações agrícolas e de construção civil.

**Características principais:**
- Processamento automático com templates pré-configurados
- Relatórios de qualidade detalhados
- Suporte a imagens RGB e multiespectrais
- Processamento em nuvem disponível
- Integração com plataformas GIS

#### DJI Terra

O **DJI Terra** é o software de mapeamento desenvolvido pela DJI, otimizado para uso com drones da marca. Oferece integração nativa e processamento eficiente.

**Características principais:**
- Integração perfeita com drones DJI
- Interface simplificada e intuitiva
- Processamento rápido para modelos 3D
- Ideal para usuários de ecossistema DJI
- Licenciamento por assinatura

### 3.3. Fluxo de Trabalho: Processamento Passo a Passo

#### Etapa 1: Importação das Imagens

O primeiro passo é importar as fotos capturadas durante o voo para o software de processamento. É importante verificar se todas as imagens foram corretamente importadas e se contêm os metadados de geolocalização (coordenadas GPS).

**Verificações importantes:**
- Número de imagens corresponde ao esperado
- Metadados EXIF presentes (coordenadas, altitude, modelo da câmera)
- Qualidade das imagens (foco, exposição, ausência de motion blur)

#### Etapa 2: Alinhamento de Fotos

Nesta etapa, o software identifica pontos comuns entre as imagens e calcula a posição e orientação de cada foto no espaço tridimensional. O resultado é uma **nuvem de pontos esparsa** e a posição estimada das câmeras.

**Parâmetros importantes:**
- **Precisão (Accuracy):** Alta para projetos profissionais
- **Pré-seleção de pares (Pair preselection):** Genérica ou por referência
- **Limite de pontos chave (Key point limit):** 40.000 a 60.000
- **Limite de pontos de amarração (Tie point limit):** 4.000 a 10.000

#### Etapa 3: Otimização e Pontos de Controle (Opcional)

Para aumentar a precisão absoluta do modelo, é possível inserir **pontos de controle** medidos em campo com GPS de precisão ou estação total. Esses pontos são identificados nas fotos e suas coordenadas reais são inseridas no software.

**Benefícios dos pontos de controle:**
- Maior precisão posicional (centimétrica)
- Correção de distorções sistemáticas
- Validação da qualidade do processamento

#### Etapa 4: Geração da Nuvem de Pontos Densa

A partir do alinhamento, o software densifica a nuvem de pontos, gerando milhões de pontos 3D que representam a superfície dos objetos. Esta é a etapa mais demorada e que exige maior capacidade computacional.

**Parâmetros importantes:**
- **Qualidade (Quality):** Alta ou Ultra Alta para projetos profissionais
- **Filtragem de profundidade (Depth filtering):** Moderada ou Agressiva

#### Etapa 5: Geração de Malha 3D e Textura

A malha 3D é uma superfície triangular gerada a partir da nuvem de pontos densa. Em seguida, as cores das fotos originais são aplicadas sobre a malha, criando um modelo 3D texturizado e realista.

**Tipos de malha:**
- **Arbitrary:** Para objetos complexos e irregulares
- **Height field:** Para terrenos e superfícies planas

#### Etapa 6: Geração de Produtos Cartográficos

**Ortofoto:**
- Imagem aérea corrigida geometricamente
- Cada pixel possui coordenadas reais
- Pode ser sobreposta a mapas e plantas
- Formato: GeoTIFF, JPEG com world file

**Modelo Digital de Superfície (MDS):**
- Representa a elevação da superfície, incluindo edificações e vegetação
- Formato: GeoTIFF, XYZ

**Modelo Digital de Terreno (MDT):**
- Representa apenas o terreno, removendo edificações e vegetação
- Requer classificação de pontos

### 3.4. Análise e Comparação entre Projeto e Execução

Uma das principais aplicações da fotogrametria na fiscalização de obras é a comparação entre o que foi projetado e o que foi efetivamente executado. Essa análise permite identificar desvios, inconformidades e subsidiar decisões técnicas.

#### Sobreposição de Plantas

A ortofoto gerada pode ser sobreposta à planta do projeto em um software CAD ou GIS. Essa sobreposição visual permite identificar rapidamente:
- Elementos construídos fora da posição prevista
- Dimensões diferentes do projeto
- Áreas não executadas
- Elementos adicionais não previstos

#### Cálculo de Volumes

O modelo 3D permite calcular volumes de terraplenagem, aterros, cortes e materiais estocados. O software compara o modelo atual com um modelo de referência (terreno original ou projeto) e calcula a diferença volumétrica.

**Aplicações:**
- Medição de volumes de escavação e aterro
- Quantificação de materiais (brita, areia, concreto)
- Acompanhamento de avanço físico de terraplenagem

#### Medição de Áreas e Distâncias

Diretamente na ortofoto ou no modelo 3D, é possível medir:
- Áreas de pavimentação, cobertura, lajes
- Distâncias lineares entre pontos
- Perímetros de edificações
- Comprimentos de vias e muros

## Atividades Práticas

### Laboratório 1: Processamento Completo em Agisoft Metashape

**Objetivo:** Processar um conjunto de imagens de drone e gerar ortofoto e modelo 3D

**Passos:**
1. Importar imagens fornecidas pelo instrutor
2. Alinhar fotos (nuvem esparsa)
3. Gerar nuvem de pontos densa
4. Gerar malha 3D e textura
5. Gerar ortofoto e MDS
6. Exportar produtos

### Laboratório 2: Análise Comparativa

**Objetivo:** Comparar ortofoto gerada com planta do projeto

**Passos:**
1. Importar ortofoto em software GIS (QGIS)
2. Sobrepor planta do projeto
3. Identificar inconformidades
4. Gerar relatório com anotações

### Laboratório 3: Cálculo de Volumes

**Objetivo:** Calcular volume de material estocado

**Passos:**
1. Definir plano de referência
2. Calcular volume acima do plano
3. Gerar relatório com resultado

## Materiais de Apoio

- Tutoriais em vídeo dos softwares
- Conjunto de imagens de exemplo
- Plantas de projeto para comparação
- Guias de boas práticas de processamento

## Avaliação

- Qualidade dos produtos gerados (ortofoto, modelo 3D)
- Precisão das medições realizadas
- Capacidade de identificar inconformidades
- Relatório técnico do processamento

