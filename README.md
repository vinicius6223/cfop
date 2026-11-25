CFOP Coach

Aplicação web single-file para treino de cubo mágico 3×3 no método CFOP, reunindo visualizador 3D com mãos articuladas, Academy interativa, Timer compatível com csTimer, Trainer de reconhecimento, gerador de scrambles, diagnóstico de erros e integração Bluetooth com cubos smart GAN.

Funcionalidades

Visualizador 3D

Categorias organizadas na ordem do solve: 2-Look OLL (10), 2-Look PLL (6), F2L Intuitivo (12), Triggers (8), além das tabelas completas Full F2L (41), Full OLL (57) e Full PLL (21).

Seletor de algoritmos alternativos direto no painel da sequência.

Mãos 3D articuladas com controle de opacidade, setas de destino no passo inicial (passo 0), destaque luminoso nas peças movimentadas e slider de zoom.

Academy

Separação mental entre OLL e PLL e tabela de combos de aprendizado (ex.: T ↔ L, U → L, Y Perm = OLL 37 + OLL 33, Ua ↔ Ub, Sune ↔ Antisune).

Rota de Fuga dinâmica: marque os casos que você já domina para calcular rotas verificadas (1 a 3 passos) para os casos restantes.

Setup de F2L (41 → 2): guia visual das mecânicas fundamentais de Split Direto e Par Pronto.

Timer & Stats

Scrambles 3×3 WCA (20 giros) e scrambles parciais (F2L, 2-Look OLL, 2-Look PLL e Last Layer).

Múltiplas sessões, cálculo de PB, Média, Ao5, Ao12, Melhor Ao5, gráfico de tendência, modo digitação, inspeção opcional de 15s (com alertas de voz opcionais) e exportação em CSV no formato csTimer.

Aba Stats unificada com métricas do Timer, desempenho por algoritmo, perfil local com PIN e Backup/Restauração completo em .json.

Cubo Smart Bluetooth (GAN Gen2 / Gen3 / Gen4)

Conexão via Web Bluetooth API utilizando gan-web-bluetooth (compatível com GAN i4, GAN14 ui, GAN12 ui, GAN356 i3 / Carry 2 e outros).

Auto-start no primeiro giro e auto-stop automático ao resolver o cubo, com contagem de movimentos e TPS ao vivo.

Espelhamento de movimentos e giroscópio 360° em tempo real no Visualizador 3D (com botão de calibração).

Reconhecimento, Trainer, Scrambles & Diagnóstico

Diagramas 2D de OLL, PLL e F2L, treino cronometrado de reconhecimento e rota de fuga, gerador de scrambles filtrados e simulador de diagnóstico para identificar erros de execução.

Como publicar no GitHub Pages

Renomeie o arquivo principal para index.html e envie para o repositório no GitHub (junto com este README.md).

No repositório, acesse Settings → Pages.

Em Build and deployment, selecione Deploy from a branch, escolha a branch main e a pasta / (root), e salve.

Acesse a URL gerada (https://<seu-usuario>.github.io/<seu-repositorio>/).

Os dados de sessões, tempos, algoritmos aprendidos e configurações ficam salvos no localStorage do navegador. Use Stats → Backup (.json) para transferir seu histórico entre dispositivos.

Requisitos para Cubo Bluetooth

Navegador baseado em Chromium com suporte a Web Bluetooth (Google Chrome ou Microsoft Edge no desktop ou Android) acessando via HTTPS (como o GitHub Pages).

Cubos GAN utilizam criptografia BLE baseada no endereço MAC. Caso o navegador solicite o MAC na primeira conexão, informe-o no campo do modal Cubo BT (ele fica salvo localmente) ou ative a flag chrome://flags/#enable-web-bluetooth-new-permissions-backend.

Tecnologias

HTML5 single-file (zero build)

Tailwind CSS

Three.js

gan-web-bluetooth
