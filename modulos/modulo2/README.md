# Módulo 2: Planejamento e Execução de Voo

**Carga Horária:** 6 horas  
**Tipo:** Teórico-Prático

## Objetivos de Aprendizagem

Ao final deste módulo, o participante será capaz de:

- Realizar análise de risco e avaliar condições de segurança para operação
- Planejar missões automatizadas utilizando aplicativos especializados
- Configurar parâmetros de voo adequados para fiscalização de obras
- Executar voos de inspeção com segurança e eficiência
- Aplicar checklists de pré-voo e pós-voo

## Conteúdo

### 2.1. Segurança Operacional

#### Análise de Risco

A segurança operacional é o pilar fundamental de qualquer operação com drones. Antes de cada voo, é essencial realizar uma análise criteriosa dos riscos envolvidos, considerando fatores como a presença de pessoas, edificações, linhas de transmissão, aeroportos e outras aeronaves.

**Matriz de Risco:**

| Probabilidade | Severidade Baixa | Severidade Média | Severidade Alta |
|:---|:---:|:---:|:---:|
| **Alta** | Médio | Alto | Crítico |
| **Média** | Baixo | Médio | Alto |
| **Baixa** | Muito Baixo | Baixo | Médio |

#### Áreas Restritas e Controladas

O espaço aéreo brasileiro é dividido em diferentes classes, e algumas áreas possuem restrições para operação de drones. É fundamental consultar o sistema SARPAS antes de qualquer voo para verificar se a área está liberada ou se é necessária autorização prévia.

**Principais restrições:**
- Proximidade de aeroportos (raio de segurança)
- Áreas militares e instalações sensíveis
- Áreas urbanas densamente povoadas
- Eventos com aglomeração de pessoas

#### Condições Meteorológicas

As condições climáticas impactam diretamente a segurança e a qualidade dos dados coletados. É necessário avaliar:

- **Vento:** Velocidade e rajadas (limite operacional do drone)
- **Chuva:** Evitar voos sob chuva (risco de danos ao equipamento)
- **Visibilidade:** Necessária para manter contato visual (VLOS)
- **Temperatura:** Impacta a autonomia da bateria

### 2.2. Planejamento de Missão Automatizada

O planejamento adequado da missão é crucial para garantir a cobertura completa da área de interesse e a qualidade dos dados coletados. Diversos aplicativos facilitam esse processo, permitindo definir rotas automatizadas.

#### Aplicativos de Planejamento

**DJI Pilot / DJI Pilot 2:**
- Integrado aos drones DJI
- Interface intuitiva
- Planejamento de rotas e waypoints

**Pix4D Capture:**
- Especializado em fotogrametria
- Cálculo automático de parâmetros
- Compatível com diversos drones

**DroneDeploy:**
- Plataforma web e mobile
- Planejamento e processamento integrados

#### Parâmetros de Voo

**Altitude de Voo:**
- Define a resolução espacial (GSD - Ground Sample Distance)
- Maior altitude = menor resolução, maior área coberta
- Menor altitude = maior resolução, menor área coberta
- Típico para obras: 30 a 80 metros

**GSD (Ground Sample Distance):**
- Distância representada por cada pixel da imagem
- Exemplo: GSD de 2 cm/pixel significa que cada pixel representa 2 cm no terreno
- Para fiscalização de obras: 1 a 3 cm/pixel

**Sobreposição de Imagens:**
- **Frontal (Forward Overlap):** 70% a 80%
- **Lateral (Side Overlap):** 60% a 70%
- Maior sobreposição = melhor qualidade do modelo 3D

**Velocidade de Voo:**
- Influencia a nitidez das imagens
- Muito rápido pode causar motion blur
- Típico: 3 a 8 m/s

### 2.3. Configuração do Drone e Checklist

#### Configuração da Câmera

- **Modo de captura:** Intervalo de tempo ou por distância
- **Formato:** JPEG (menor tamanho) ou RAW (maior qualidade)
- **Exposição:** Ajuste conforme iluminação (evitar sub ou superexposição)
- **Foco:** Infinito (para evitar desfoque)

#### Checklist Pré-Voo

**Equipamento:**
- [ ] Bateria do drone carregada (100%)
- [ ] Baterias reserva carregadas
- [ ] Bateria do controle remoto carregada
- [ ] Cartão de memória formatado e com espaço suficiente
- [ ] Hélices em bom estado e corretamente instaladas
- [ ] Firmware atualizado

**Planejamento:**
- [ ] Missão planejada e carregada no aplicativo
- [ ] Autorização SARPAS obtida (se necessário)
- [ ] Condições meteorológicas verificadas
- [ ] Área de decolagem e pouso identificada

**Segurança:**
- [ ] Pessoas afastadas da área de operação
- [ ] Obstáculos identificados
- [ ] Plano de contingência definido

#### Checklist Pós-Voo

- [ ] Verificar integridade física do drone
- [ ] Verificar número de fotos capturadas
- [ ] Fazer backup das imagens
- [ ] Registrar dados do voo (log)
- [ ] Limpar equipamento
- [ ] Recarregar baterias

### 2.4. Execução Prática de Voo

#### Decolagem

- Posicionar o drone em superfície plana e estável
- Aguardar conexão com satélites GPS (mínimo 10 satélites)
- Verificar calibração da bússola e IMU
- Iniciar motores e decolar suavemente

#### Durante o Voo

- Monitorar constantemente o drone
- Acompanhar telemetria (bateria, altitude, distância)
- Observar condições meteorológicas
- Estar preparado para assumir controle manual se necessário

#### Pouso

- Retornar ao ponto de decolagem (RTH - Return to Home)
- Pousar suavemente
- Desligar motores somente após o pouso completo

## Atividades Práticas

1. **Laboratório:** Planejamento de missão em software
   - Definir área de interesse
   - Calcular parâmetros de voo
   - Gerar rota automatizada

2. **Campo:** Execução de voo de inspeção
   - Aplicar checklist pré-voo
   - Executar missão planejada
   - Coletar imagens de uma obra ou estrutura

## Materiais de Apoio

- Manual do usuário do drone utilizado
- Tutoriais dos aplicativos de planejamento
- Checklist impresso para uso em campo

## Avaliação

- Qualidade do planejamento da missão
- Execução segura do voo prático
- Aplicação correta dos checklists
- Qualidade das imagens coletadas

