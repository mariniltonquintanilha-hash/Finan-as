# Finanças

🚀 Funcionalidades Principais
📊 Dashboard Inteligente
Visão Geral Financeira: Receitas, despesas e lucro líquido em tempo real

Gráficos Dinâmicos: Visualização interativa com Chart.js

Atualização Automática: Dados atualizados instantaneamente com novos registros

💰 Gestão de Transações
Registro Completo: Adicione receitas e despesas com descrição, valor e data

Filtros Avançados:

Por tipo (receita/despesa)

Por mês específico

Por data específica

Edição em Tempo Real: Modifique registros existentes

Exclusão Segura: Remova registros com confirmação

📈 Análise Financeira
Balanço Automático: Cálculo instantâneo do lucro líquido

Histórico Completo: Todos os registros organizados em tabela

Período dos 30 dias: Foco no último mês para análise relevante

🔄 Exportação de Dados
Excel/CSV: Exporte todos os registros para planilha

Formato XLSX: Compatível com Excel, Google Sheets e outros

Dados Estruturados: Mantém todas as informações e formatações

🛠️ Tecnologias Utilizadas
Frontend
HTML5 - Estrutura semântica moderna

CSS3 - Estilização com variáveis CSS e Flexbox/Grid

JavaScript Vanilla - Lógica da aplicação

Bibliotecas Externas
Chart.js (v3.9.1) - Gráficos interativos e responsivos

SheetJS/xlsx (v0.17.0) - Exportação para Excel

Google Fonts - Tipografia moderna (Roboto + Orbitron)

🎯 Características Técnicas
Sistema de Design Futurista
Paleta de Cores:

Primária: #00d8ff (Ciano neon)

Fundo: #0a192f (Azul escuro)

Cards: #172a45 (Azul acinzentado)

Sucesso: #00ff88 (Verde neon)

Alerta: #ff6b6b (Vermelho)

Tipografia:

Títulos: Orbitron (futurista, peso 400-700)

Texto: Roboto (legível, peso 300-700)

Efeitos Visuais:

Animações suaves (pulse, glow)

Transições em hover

Cards com sombras neon

Design glassmorphism

Estrutura de Arquivos
text
quantum-mei/
│
├── index.html              # Página principal
│
├── css/
│   └── styles.css          # Estilos principais
│
├── js/
│   └── script.js           # Lógica da aplicação
│
├── assets/                 # (Opcional) Imagens e ícones
│
└── README.md               # Documentação
Componentes da Interface
Dashboard Header

Título com efeito glow

Subtítulo explicativo

Cards de Métricas (3 colunas)

Receitas Totais (30 dias)

Despesas Totais (30 dias)

Lucro Líquido (atual)

Gráfico Financeiro

Linha temporal interativa

Diferenciação por cores

Legenda clara

Formulário de Registro

Campos: Descrição, Valor, Data, Tipo

Validação em tempo real

Botão com efeito hover

Seção de Filtros

Filtro por data específica

Filtro por tipo (receita/despesa)

Filtro por mês

Botões de aplicar/limpar

Tabela de Registros

Colunas: Data, Descrição, Valor, Tipo, Ações

Paginação implícita via rolagem

Botões de editar/excluir por linha

Controles de Exportação

Botão para exportar Excel

Posicionamento intuitivo

📱 Responsividade
Desktop (≥1024px): Layout em grid completo

Tablet (768px-1023px): Cards em 2 colunas

Mobile (<768px): Single column, menu adaptativo

Touch-friendly: Botões e inputs ampliados para mobile

🚀 Como Executar
Método 1: Localmente
bash
# Clone o repositório
git clone [seu-repositorio]

# Navegue até a pasta
cd quantum-mei

# Abra o arquivo principal
# Execute em qualquer servidor local ou abra diretamente no navegador
Método 2: Servidor Local (Recomendado)
bash
# Com Python
python -m http.server 8000

# Com Node.js (http-server)
npx http-server

# Com PHP
php -S localhost:8000
Método 3: GitHub Pages
Faça push para o repositório

Ative GitHub Pages nas configurações

Acesse: https://[seu-usuario].github.io/quantum-mei

🔧 Configuração e Personalização
Modificando Cores
Edite as variáveis CSS em css/styles.css:

css
:root {
    --primary-color: #00d8ff;
    --secondary-color: #0a192f;
    --success-color: #00ff88;
    /* Personalize conforme necessidade */
}
Adicionando Novos Campos
Para adicionar novos campos ao formulário:

Adicione no HTML:

html
<div class="form-group">
    <label for="novoCampo">Novo Campo</label>
    <input type="text" id="novoCampo" placeholder="Descrição">
</div>
Atualize a lógica em script.js:

javascript
const novoCampo = document.getElementById('novoCampo').value;
// Adicione ao objeto de registro
Customizando o Gráfico
Acesse a configuração do Chart.js em script.js:

javascript
const chartConfig = {
    type: 'line',  // Pode ser 'bar', 'pie', etc.
    options: {
        // Personalize animações, legendas, etc.
    }
}
📊 Armazenamento de Dados
Local Storage
Os dados são persistidos automaticamente no localStorage do navegador:

Chave: quantumMeiRecords

Formato: Array de objetos JSON

Backup automático: Sempre que há alterações

Estrutura dos Registros
javascript
{
    id: "unique-id",
    description: "Descrição da transação",
    value: 150.50,
    date: "2024-01-15",
    type: "renda" // ou "gastos"
}
🔒 Segurança e Boas Práticas
Validação de Entrada: Todos os campos são validados

Sanitização: Prevenção contra XSS básico

Local Storage: Dados apenas no cliente

Responsividade: Funciona offline após carregamento

📱 Compatibilidade
Navegadores Suportados
✅ Chrome 60+

✅ Firefox 55+

✅ Safari 11+

✅ Edge 79+

✅ Opera 50+

Requisitos do Sistema
JavaScript habilitado

Conexão inicial para carregar bibliotecas

10MB de espaço livre (para dados)

Resolução mínima: 320px

🚨 Limitações Conhecidas
Armazenamento: Limitado a ~5MB por domínio

Offline: Requer conexão para carregar recursos externos

Backup: Sem backup automático em nuvem

Multi-usuário: Apenas para uso individual

🔄 Roadmap (Futuras Melhorias)
Autenticação de usuários

Sincronização em nuvem

Relatórios PDF

Notificações por e-mail

Integração com APIs bancárias

App móvel (PWA)

Categorias personalizadas

Meta de economias

🤝 Como Contribuir
Fork o projeto

Crie uma branch (git checkout -b feature/nova-funcionalidade)

Commit suas mudanças (git commit -m 'Adiciona nova funcionalidade')

Push para a branch (git push origin feature/nova-funcionalidade)

Abra um Pull Request



